# 깃 커밋 취소하기
```shell
git reset HEAD^ # 최종 커밋을 취소. 워킹트리는 보존됨. (커밋은 했으나 push하지 않은 경우)
git reset HEAD~2 # 마지막 두개의 커밋을 취소. 워킹트리는 보존됨.
git reset --hard HEAD~2 # 마지막 2개의 커밋을 취소. index 및 워킹트리 모두 원복됨.
git reset --hard ORIG_HEAD # 머지한 것을 이미 커밋했을 때,  그 커밋을 취소. (잘못된 머지를 이미 커밋한 경우 유용)
git revert HEAD # HEAD에서 변경한 내역을 취소하는 새로운 커밋 발행(undo commit). (커밋을 이미 push 해버린 경우 유용)
```

## Reference
http://ecogeo.tistory.com/276
