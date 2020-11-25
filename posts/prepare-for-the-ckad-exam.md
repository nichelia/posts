# Prepare for the CKAD exam

## Exam Format

This is related to the Kubernetes exam for [Certified Kubernetes Application Developer (CKAD)](https://www.cncf.io/certification/ckad/).

* Exam questions are all practice based (command line in a real kubernetes cluster).
* Kubernetes version can change - often updates every 3 months.
* Exam is comprised of 15-20 tasks of different weight. Can be attempted in any order.
* Duration 2 hours.
* Pass rate 66% (includes a free retake)
* Open Book: Urls allowed are:
    * [https://kubernetes.io/docs/](https://kubernetes.io/docs/)
    * [https://github.com/kubernetes/](https://github.com/kubernetes/)
    * [https://kubernetes.io/blog/](https://kubernetes.io/blog/)

## Candidate Information

* [Linux Foundation Certification Exams: Candidate Handbook](https://docs.linuxfoundation.org/tc-docs/certification/lf-candidate-handbook)
* [Curriculum](https://github.com/cncf/curriculum)
* [Instructions](https://docs.linuxfoundation.org/tc-docs/certification/tips-cka-and-ckad)
* [FAQ](https://docs.linuxfoundation.org/tc-docs/certification/faq-cka-ckad-cks)
* [Agreement](https://docs.linuxfoundation.org/tc-docs/certification/lf-cert-agreement/)
* [Verification](https://training.linuxfoundation.org/certification/verify/)

## Tips

1. Attach autocomplete to the terminal's shell: `source <(kubectl completion bash)`.
2. Make use of `tmux`. This will enable more screen estate within the one terminal window.
   Useful commands: 
    * `CTRL+b %` to split window vertically
    * `CTRL+b "` to split window horizontally
    * `CTRL+b arrows(up,down,left,right)` to move between panes
    * `CTRL+b x` to close plane
3. Use the `kubetl <command> --help | more/grep` util of each command. This will show information of the command.
4. Use the `kubectl explain <object>` util for objects.

## Useful commands

* Events: `kubectl get events`
* Logs: `kubectl logs <pod_name> --follow`
* Generate manifests: 
    * `kubectl run --image=<image_name> <name> --dry-run=client -o yaml > <output>.pod.yaml`
    * `kubectl create deployment <name> --image=<image_name> --dry-run=client -o yaml > <output>.deployment.yaml`
* Copy/Paste manifests:
    ```bash
    cat << eof > file.yaml
    <content_here>
    eof
    ```
* Edit manifests: `vim <file>.yaml`
* Apply manifests: 
    ```bash
    cat << eof | kubectl apply -f -
    <content_here>
    eof
    ```
* Edit using cli: `kubectl edit <resource> <name>`
* Switch namespace in context: `kubectl config set-context --current --namespace=<namespace_name>`
* Update resources: `kubectl set`, `kubectl rollout`
* Executing in pod: `kubectl exec -it <pod_name> -- <cmd>`

## Practice

* [CKAD Exercises](https://github.com/dgkanatsios/CKAD-exercises)
* [Practice Enough With These 150 Questions for the CKAD Exam](https://medium.com/bb-tutorials-and-thoughts/practice-enough-with-these-questions-for-the-ckad-exam-2f42d1228552)

## Benchmarks

[CKAD](https://raw.githubusercontent.com/nichelia/posts/main/assets/prepare-for-the-ckad-exam/CKAD_benchmarks.html)

## References

* [How I passed the CKA (Certified Kubernetes Administrator) Exam](https://medium.com/platformer-blog/how-i-passed-the-cka-certified-kubernetes-administrator-exam-8943aa24d71d)
* [Cloud Academy: Office Hours | Hands-on Tips to Pass the CKAD Exam](https://www.youtube.com/watch?v=L6K_8dOFR5w&t=1186s)
* [ckad-prep-notes](https://github.com/twajr/ckad-prep-notes)

---
Cover photo: [@spathumpa](https://www.instagram.com/p/B16_56joHX3/?igshid=yc35apjmrj60)
