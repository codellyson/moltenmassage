<script>
  const testimonies = [
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 1,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 2,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 3,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
    {
      image: "images/founder.jpg",
      name: "Lastname Firstname",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
  ];
  const spa_features = [
    {
      icon:
        "data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjUxMiIgdmlld0JveD0iMCAwIDYwIDU2IiB3aWR0aD0iNTEyIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxnIGlkPSJQYWdlLTEiIGZpbGw9Im5vbmUiIGZpbGwtcnVsZT0iZXZlbm9kZCI+PGcgaWQ9IjAyMy0tLUNsZWFuLVRvd2VscyIgZmlsbD0icmdiKDAsMCwwKSIgZmlsbC1ydWxlPSJub256ZXJvIj48cGF0aCBpZD0iU2hhcGUiIGQ9Im02MCAxNWMtLjAwNDQwODYtMy44NjQxNjU3LTMuMTM1ODM0My02Ljk5NTU5MTM2LTctN2gtMzBjLS42MTM5ODk0LS4wMDIxODU4OC0xLjIyNTI1OTUuMDgxNjI4MTQtMS44MTYuMjQ5LS4zNzQuMDktMTAuMjUyIDMuODE0LTE2LjEwNyA2LjAyNWgtLjAwOGMtMS4xNDExNjYzOC4zMTg0NzgxLTIuMTc5NjI4MDIuOTI4ODcxNi0zLjAxMyAxLjc3MS0xLjMyMzgwNzkyIDEuMzA3OTU5MS0yLjA2NDkxNzM5IDMuMDk0MDQ3My0yLjA1NiA0Ljk1NS4wMDE2NTk5OCAyLjQ2MDE5NTMgMS4yOTU3OTE2OSA0LjczODU5NjIgMy40MDggNi0yLjExMTMyNDM5IDEuMjYyMjY4NS0zLjQwNTE0NDY3IDMuNTQwMTIxMS0zLjQwOCA2IC4wMDM5MDcyOCAyLjQ2MDg4OTkgMS4yOTk3NTU4OSA0LjczODk3MTIgMy40MTMgNi0yLjcwNDM5NzM1IDEuNjExODQwNi0zLjk5ODI3MzQyIDQuODMyMTM2MS0zLjE2MDg3NyA3Ljg2NzAyNjkuODM3Mzk2NDIgMy4wMzQ4OTA5IDMuNTk5NTc4MTEgNS4xMzYwMjY0IDYuNzQ3ODc3IDUuMTMyOTczMWgzMGMxLjAzNDU4MjctLjAwMDg3NTMgMi4wNTU4NjE3LS4yMzMyMTcxIDIuOTg5LS42OC4wMDczMjU2LjAwMDQ3NS4wMTQ2NzQ0LjAwMDQ3NS4wMjIgMGwxNi4wODktNi4wNDNjMi4yOTc3MTU1LTEuMTMxOTQwNiAzLjc5MTQ0MzQtMy40MzA4NDg2IDMuODkyMjA5Ni01Ljk5MDI2ODlzLTEuMjA3NTk4OS00Ljk2ODY0ODctMy40MDkyMDk2LTYuMjc3NzMxMWMuNDk5MDE1Ni0uMjg5MjA5MS45NTYyMzMzLS42NDUxNTkzIDEuMzU5LTEuMDU4IDEuMzIzNTQ4NS0xLjMwNjY1NDMgMi4wNjUzMTI4LTMuMDkxMTQxOCAyLjA1OC00Ljk1MS0uMDA4NzQ4OS0yLjQ1NzI0NzEtMS4zMDIyMjk5LTQuNzMwODkwOC0zLjQxLTUuOTk0LjQ5NjgwOTItLjI4OTA0OTguOTUyMjY2MS0uNjQzOTI5NCAxLjM1NC0xLjA1NSAxLjMyMjgxNDMtMS4zMDY5ODY5IDIuMDYzODQwNC0zLjA5MTQzMjYgMi4wNTYtNC45NTF6bS0zOC4yNjUtNC44MjljLjQxMTc1OTMtLjExNTA4MjQuODM3NDY0LS4xNzI2MjgyMyAxLjI2NS0uMTcxaDMwYzIuNzYwMDUzMi4wMDMzMDYxIDQuOTk2NjkzOSAyLjIzOTk0NjggNSA1IC4wMDYxMjYyIDEuMzI3MDUwMi0uNTIyNjg2NiAyLjYwMDU5ODgtMS40NjcgMy41MzMtLjMzOTc1MjEuMzUzNjExNS0uNzM3NDg3Ni42NDY1MDE3LTEuMTc2Ljg2Ni0uMDU0LjAyOS0uMS4wNTYtLjE1MS4wODItMS4zNDkuNS0zLjcyNCAxLjM5Mi03LjQwNSAyLjc3NGwtNC40NDQgMS42NjljLjk5OTAyNjgtMi4xNjY2Mjg5LjgyNDg0MzgtNC42OTMwMzIzLS40NjIwNzM2LTYuNzAyMDU2N3MtMy41MDkwNjU0LTMuMjIzNTY2My01Ljg5NDkyNjQtMy4yMjE5NDMzaC0yNS41MjhjNC45NzktMS44NzUgOS44NTYtMy43IDEwLjI2My0zLjgyOXptLTE5LjczNSAxMC44MjljLS4wMDU3MDE5Ny0xLjMyOTQyMDguNTI0OTkxMDItMi42MDQ5NTg3IDEuNDcyLTMuNTM4LjYwNDQ1MDA5LS42MTM2ODU5IDEuMzYyNDU5NDMtMS4wNTM5ODc1IDIuMTk1LTEuMjc1LjAyNS0uMDA4LjA1NC0uMDE3LjA4My0uMDI4LjQwODAyNTA3LS4xMDY4OTcyLjgyODIwNjYxLS4xNjAzNDQzIDEuMjUtLjE1OWgzMGMyLjc2MDA1MzIuMDAzMzA2MSA0Ljk5NjY5MzkgMi4yMzk5NDY4IDUgNS0uMDA3Mjc5MiAxLjg3MDg4MjktMS4wNTEzMTE4IDMuNTgzNDY2LTIuNzExIDQuNDQ3LS4wMjkyODQ1LjAxMTIxOTUtLjA1Nzk4NzMuMDIzOTAyMi0uMDg2LjAzOC0uNjgzNzc1Ny4zNDIwNzk2LTEuNDM4NDM3Ny41MTg0OTg2LTIuMjAzLjUxNWgtMzBjLTIuNzYwMDUzMTUtLjAwMzMwNjEtNC45OTY2OTM4OC0yLjIzOTk0NjgtNS01em0wIDEyYy4wMDQ5NTM1LTIuNzU5MzY5MyAyLjI0MDYzMDY2LTQuOTk1MDQ2NSA1LTVoMzBjMi43NjAwNTMyLjAwMzMwNjEgNC45OTY2OTM5IDIuMjM5OTQ2OCA1IDUtLjAwNzI3OTIgMS44NzA4ODI5LTEuMDUxMzExOCAzLjU4MzQ2Ni0yLjcxMSA0LjQ0Ny0uMDI5Mjg0NS4wMTEyMTk1LS4wNTc5ODczLjAyMzkwMjItLjA4Ni4wMzgtLjY4Mzc3NTcuMzQyMDc5Ni0xLjQzODQzNzcuNTE4NDk4Ni0yLjIwMy41MTVoLTMwYy0yLjc2MDA1MzE1LS4wMDMzMDYxLTQuOTk2NjkzODgtMi4yMzk5NDY4LTUtNXptNSAxN2MtMi43NjE0MjM3NSAwLTUtMi4yMzg1NzYzLTUtNXMyLjIzODU3NjI1LTUgNS01aDMwYzIuNzYxNDIzNyAwIDUgMi4yMzg1NzYzIDUgNXMtMi4yMzg1NzYzIDUtNSA1em01MS0xMWMuMDA2MDUwNSAxLjMyNjgzNzktLjUyMjM0MDggMi42MDAyMzkyLTEuNDY2IDMuNTMzLS4zNTk1NDIzLjM2NDAyMzItLjc3MjY1MzMuNjcwOTA1Ny0xLjIyNS45MWwtMTEuOTU5IDQuNDg1YzEuNDkwMTgzNS0zLjIwMjQ4NDEuMzQ2MzkzNi03LjAxMzM5NzctMi42NjEtOC44NjZsMTMuMi00Ljk1MmMyLjM3MTUzODUuNDIzMTM3MiA0LjEwMTU5NjcgMi40ODEwMjY5IDQuMTExIDQuODl6bTAtMTJjLjAwNjEyNjIgMS4zMjcwNTAyLS41MjI2ODY2IDIuNjAwNTk4OC0xLjQ2NyAzLjUzMy0uMzM5NzUyMS4zNTM2MTE1LS43Mzc0ODc2LjY0NjUwMTctMS4xNzYuODY2LS4wNTUuMDMtLjEwNy4wNTctLjE1My4wODNsLTExLjg0OCA0LjQ0M2MxLjQ4MTA1NjYtMy4yMDM2MjI4LjMzNjA1MzUtNy4wMDg3MDgzLTIuNjY3LTguODYzbDcuODExLTIuOTM0YzIuMjgyLS44NTcgNC4wNTUtMS41MjMgNS40LTIuMDI2IDIuMzY3MzM4OC40MzMxNzYgNC4wOTAyMDk1IDIuNDkxMzc2MSA0LjEgNC44OTh6Ii8+PHBhdGggaWQ9IlNoYXBlIiBkPSJtMzkgMjFjMC0uNTUyMjg0Ny0uNDQ3NzE1My0xLTEtMWgtMzJjLS41NTIyODQ3NSAwLTEgLjQ0NzcxNTMtMSAxcy40NDc3MTUyNSAxIDEgMWgzMmMuNTUyMjg0NyAwIDEtLjQ0NzcxNTMgMS0xeiIvPjxwYXRoIGlkPSJTaGFwZSIgZD0ibTM5IDMzYzAtLjU1MjI4NDctLjQ0NzcxNTMtMS0xLTFoLTMyYy0uNTUyMjg0NzUgMC0xIC40NDc3MTUzLTEgMXMuNDQ3NzE1MjUgMSAxIDFoMzJjLjU1MjI4NDcgMCAxLS40NDc3MTUzIDEtMXoiLz48cGF0aCBpZD0iU2hhcGUiIGQ9Im0zOCA0NGgtMzJjLS41NTIyODQ3NSAwLTEgLjQ0NzcxNTMtMSAxcy40NDc3MTUyNSAxIDEgMWgzMmMuNTUyMjg0NyAwIDEtLjQ0NzcxNTMgMS0xcy0uNDQ3NzE1My0xLTEtMXoiLz48cGF0aCBpZD0iU2hhcGUiIGQ9Im0xMCAwYy0uNTUyMjg0NzUgMC0xIC40NDc3MTUyNS0xIDF2MmMwIC41NTIyODQ3NS40NDc3MTUyNSAxIDEgMSAuNTUyMjg0NyAwIDEtLjQ0NzcxNTI1IDEtMXYtMmMwLS41NTIyODQ3NS0uNDQ3NzE1My0xLTEtMXoiLz48cGF0aCBpZD0iU2hhcGUiIGQ9Im05IDljMCAuNTUyMjg0NzUuNDQ3NzE1MjUgMSAxIDEgLjU1MjI4NDcgMCAxLS40NDc3MTUyNSAxLTF2LTJjMC0uNTUyMjg0NzUtLjQ0NzcxNTMtMS0xLTEtLjU1MjI4NDc1IDAtMSAuNDQ3NzE1MjUtMSAxeiIvPjxwYXRoIGlkPSJTaGFwZSIgZD0ibTggNGgtMmMtLjU1MjI4NDc1IDAtMSAuNDQ3NzE1MjUtMSAxcy40NDc3MTUyNSAxIDEgMWgyYy41NTIyODQ3NSAwIDEtLjQ0NzcxNTI1IDEtMXMtLjQ0NzcxNTI1LTEtMS0xeiIvPjxwYXRoIGlkPSJTaGFwZSIgZD0ibTEyIDZoMmMuNTUyMjg0NyAwIDEtLjQ0NzcxNTI1IDEtMXMtLjQ0NzcxNTMtMS0xLTFoLTJjLS41NTIyODQ3IDAtMSAuNDQ3NzE1MjUtMSAxcy40NDc3MTUzIDEgMSAxeiIvPjxwYXRoIGlkPSJTaGFwZSIgZD0ibTU4LjIwNyA1Mi43OTNjLS4zOTIzNzg5LS4zNzg5NzIyLTEuMDE2MDg0OC0uMzczNTUyNC0xLjQwMTgxODYuMDEyMTgxNHMtLjM5MTE1MzYgMS4wMDk0Mzk3LS4wMTIxODE0IDEuNDAxODE4NmwxLjUgMS41Yy4zOTIzNzg5LjM3ODk3MjIgMS4wMTYwODQ4LjM3MzU1MjQgMS40MDE4MTg2LS4wMTIxODE0cy4zOTExNTM2LTEuMDA5NDM5Ny4wMTIxODE0LTEuNDAxODE4NnoiLz48cGF0aCBpZD0iU2hhcGUiIGQ9Im01My43OTMgNTEuMjA3Yy4zOTIzNzg5LjM3ODk3MjIgMS4wMTYwODQ4LjM3MzU1MjQgMS40MDE4MTg2LS4wMTIxODE0cy4zOTExNTM2LTEuMDA5NDM5Ny4wMTIxODE0LTEuNDAxODE4NmwtMS41LTEuNWMtLjM5MjM3ODktLjM3ODk3MjItMS4wMTYwODQ4LS4zNzM1NTI0LTEuNDAxODE4Ni4wMTIxODE0cy0uMzkxMTUzNiAxLjAwOTQzOTctLjAxMjE4MTQgMS40MDE4MTg2eiIvPjxwYXRoIGlkPSJTaGFwZSIgZD0ibTUyLjI5MyA1NS43MDdjLjM5MDQ5OTkuMzkwMzgxOSAxLjAyMzUwMDEuMzkwMzgxOSAxLjQxNCAwbDEuNS0xLjVjLjM3ODk3MjItLjM5MjM3ODkuMzczNTUyNC0xLjAxNjA4NDgtLjAxMjE4MTQtMS40MDE4MTg2cy0xLjAwOTQzOTctLjM5MTE1MzYtMS40MDE4MTg2LS4wMTIxODE0bC0xLjUgMS41Yy0uMzkwMzgxOS4zOTA0OTk5LS4zOTAzODE5IDEuMDIzNTAwMSAwIDEuNDE0eiIvPjxwYXRoIGlkPSJTaGFwZSIgZD0ibTU4LjI5MyA0OC4yOTMtMS41IDEuNWMtLjI1OTk1NjYuMjUxMDc0NS0uMzY0MjEyNi42MjI4Nzc5LS4yNzI2OTcyLjk3MjUwNzMuMDkxNTE1NS4zNDk2Mjk1LjM2NDU2MDQuNjIyNjc0NC43MTQxODk5LjcxNDE4OTkuMzQ5NjI5NC4wOTE1MTU0LjcyMTQzMjgtLjAxMjc0MDYuOTcyNTA3My0uMjcyNjk3MmwxLjUtMS41Yy4zNzg5NzIyLS4zOTIzNzg5LjM3MzU1MjQtMS4wMTYwODQ4LS4wMTIxODE0LTEuNDAxODE4NnMtMS4wMDk0Mzk3LS4zOTExNTM2LTEuNDAxODE4Ni0uMDEyMTgxNHoiLz48L2c+PC9nPjwvc3ZnPg==",
      title: "Relaxing Massage",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 1,
    },
    {
      icon:
        "data:image/svg+xml;base64,PHN2ZyBpZD0iYm93bC1jYW5kbGUiIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDMwMCAzMDAiIGhlaWdodD0iNTEyIiB2aWV3Qm94PSIwIDAgMzAwIDMwMCIgd2lkdGg9IjUxMiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48Zz48Y2lyY2xlIGN4PSIxMTgiIGN5PSI4NiIgcj0iNCIvPjxwYXRoIGQ9Im02NiA0OS41MTJjMi4yMTEgMCA0LTEuNzkxIDQtNHYtNS42NmMwLTIuMjA5LTEuNzg5LTQtNC00cy00IDEuNzkxLTQgNHY1LjY2YzAgMi4yMDkgMS43ODkgNCA0IDR6Ii8+PHBhdGggZD0ibTY2IDcyLjE0OGMyLjIxMSAwIDQtMS43OTEgNC00di01LjY2YzAtMi4yMDktMS43ODktNC00LTRzLTQgMS43OTEtNCA0djUuNjZjMCAyLjIwOSAxLjc4OSA0IDQgNHoiLz48cGF0aCBkPSJtNTEuODUyIDU4aDUuNjZjMi4yMTEgMCA0LTEuNzkxIDQtNHMtMS43ODktNC00LTRoLTUuNjZjLTIuMjExIDAtNCAxLjc5MS00IDRzMS43ODkgNCA0IDR6Ii8+PHBhdGggZD0ibTc0LjQ4OCA1OGg1LjY2YzIuMjExIDAgNC0xLjc5MSA0LTRzLTEuNzg5LTQtNC00aC01LjY2Yy0yLjIxMSAwLTQgMS43OTEtNCA0czEuNzg5IDQgNCA0eiIvPjxwYXRoIGQ9Im0yMDAgNjJjNy43MTkgMCAxNC02LjI4MSAxNC0xNHMtNi4yODEtMTQtMTQtMTQtMTQgNi4yODEtMTQgMTQgNi4yODEgMTQgMTQgMTR6bTAtMjBjMy4zMDkgMCA2IDIuNjkxIDYgNnMtMi42OTEgNi02IDYtNi0yLjY5MS02LTYgMi42OTEtNiA2LTZ6Ii8+PHBhdGggZD0ibTIxNS44MjQgMTE0LjE3NmMuNzgxLjc4MSAxLjgwNSAxLjE3MiAyLjgyOCAxLjE3MnMyLjA0Ny0uMzkxIDIuODI4LTEuMTcybDQuNTItNC41MiA0LjUyIDQuNTJjLjc4MS43ODEgMS44MDUgMS4xNzIgMi44MjggMS4xNzJzMi4wNDctLjM5MSAyLjgyOC0xLjE3MmMxLjU2Mi0xLjU2MiAxLjU2Mi00LjA5NCAwLTUuNjU2bC00LjUyLTQuNTIgNC41Mi00LjUyYzEuNTYyLTEuNTYyIDEuNTYyLTQuMDk0IDAtNS42NTZzLTQuMDk0LTEuNTYyLTUuNjU2IDBsLTQuNTIgNC41Mi00LjUyLTQuNTJjLTEuNTYyLTEuNTYyLTQuMDk0LTEuNTYyLTUuNjU2IDBzLTEuNTYyIDQuMDk0IDAgNS42NTZsNC41MiA0LjUyLTQuNTIgNC41MmMtMS41NjIgMS41NjItMS41NjIgNC4wOTMgMCA1LjY1NnoiLz48cGF0aCBkPSJtMjY2IDE2NGMwLTQuNzU0LTIuNjg0LTkuMTk1LTcuOTczLTEzLjE5OS0uMjI1LS4xNzEtLjQ4Ni0uMjM3LS43MzEtLjM1My01LjgxOC0xNC44MTctNDcuODQxLTIyLjA3Ny04NS41NjItMjMuOTI1LjAzNS0uNDkzLjE0OC0uOTYzLjE0OC0xLjQ2NCAwLTUuMDI5LTEuOTU3LTE3LjIyMS01LjEyMS0yOC4xNS00LjUyMy0xNS42My05LjU1LTIyLjkwOS0xNS44Mi0yMi45MDlzLTExLjI5NyA3LjI3OS0xNS44MiAyMi45MDhjLTMuMTY0IDEwLjkzLTUuMTIxIDIzLjEyMS01LjEyMSAyOC4xNSAwIC40NzEuMTA4LjkxMy4xMzkgMS4zNzctMzguMzczIDEuNzA2LTgxLjExNyA4Ljg1Ni04Ny4zMzkgMjMuNzczLTUuODI1IDQuMTYzLTguOCA4Ljc5OC04LjggMTMuNzkyIDAgMy43IDEuNzExIDcuMTA4IDQuNzY5IDEwLjIyOSA2LjYwNCA1Mi4zMjUgNTQuMzk4IDkxLjc3MSAxMTEuMjMxIDkxLjc3MXMxMDQuNjI3LTM5LjQ0NiAxMTEuMjMxLTkxLjc3MWMzLjA1OC0zLjEyMSA0Ljc2OS02LjUyOSA0Ljc2OS0xMC4yMjl6bS0xMTUuMTUyLTgyLjAxYzUuMTg0IDEuNDg0IDEzLjAzNSAzMS42NjIgMTMuMDM1IDQzLjA2OCAwIDcuMTM3LTUuODA1IDEyLjk0MS0xMi45NDEgMTIuOTQxcy0xMi45NDItNS44MDQtMTIuOTQyLTEyLjk0YzAtMTEuNDA3IDcuODUyLTQxLjU4NCAxMi44NDgtNDMuMDY5em0tMTguNTY1IDUyLjM3OWMyLjcyMyA1LjQyOSA3LjY4OCA5LjUwNyAxMy43MTcgMTAuOTc4djguNjUzYzAgMi4yMDkgMS43ODkgNCA0IDRzNC0xLjc5MSA0LTR2LTguMzA5YzYuODMyLTEuMDEyIDEyLjU0Ny01LjMgMTUuNTYtMTEuMjQ3IDUxLjc4OSAyLjI5OSA4MC40NCAxMi45NSA4MC40NCAxOS41NTYgMCA2Ljk4LTM0LjM0NCAyMC0xMDAgMjBzLTEwMC0xMy4wMi0xMDAtMjBjMC01LjU4NyAyNC45MS0xNy4zNSA4Mi4yODMtMTkuNjMxem0tODguMzcxIDI1LjQ0OGMxMC45MzIgMTYuMTQ4IDY3LjA1NCAyMi4xODMgMTA2LjA4OCAyMi4xODMgMzkuMDI0IDAgOTUuMTI3LTYuMDMyIDEwNi4wNzktMjIuMTcxIDEuMDk4IDEuMjcxIDEuOTIxIDIuNzAxIDEuOTIxIDQuMTcxIDAgMTAuODU3LTQxLjA4NiAyNi0xMDggMjZzLTEwOC0xNS4xNDMtMTA4LTI2YzAtMS40NjEuNzkyLTIuODkxIDEuOTEyLTQuMTgzem0xMDYuMDg4IDk4LjE4M2MtNDkuOTg0IDAtOTIuMzc1LTMyLjY1OS0xMDEuOTQ1LTc3LjEzOCAyMC45OTEgMTEuMjE3IDYyLjMyOSAxNy4xMzggMTAxLjk0NSAxNy4xMzhzODAuOTU0LTUuOTIxIDEwMS45NDUtMTcuMTM4Yy05LjU3IDQ0LjQ3OS01MS45NjEgNzcuMTM4LTEwMS45NDUgNzcuMTM4eiIvPjxwYXRoIGQ9Im0xNTAuOTQxIDEzMy4xMzVjMy4yNTYgMCA1Ljg5NS0yLjYzOSA1Ljg5NS01Ljg5NXMtMi42MzktMTYuMzc1LTUuODk1LTE2LjM3NS01Ljg5NSAxMy4xMTktNS44OTUgMTYuMzc1IDIuNjQgNS44OTUgNS44OTUgNS44OTV6Ii8+PHBhdGggZD0ibTIwMi4wMDQgMjM4Yy43NjIgMCAxLjUzMS0uMjE3IDIuMjE1LS42NzIgMTIuMzc1LTguMjUgMjguMjM0LTI3Ljk5MiAyOC45MDYtMjguODMgMS4zNzktMS43MjUgMS4wOTgtNC4yNDItLjYyNS01LjYyMS0xLjcyNy0xLjM4MS00LjI0Mi0xLjA5OC01LjYyNS42MjUtLjE1Ni4xOTUtMTUuNzQyIDE5LjYwMi0yNy4wOTQgMjcuMTctMS44NCAxLjIyNS0yLjMzNiAzLjcwOS0xLjEwOSA1LjU0Ny43NjkgMS4xNTYgMi4wMzkgMS43ODEgMy4zMzIgMS43ODF6Ii8+PC9nPjwvc3ZnPg==",
      title: "Candle",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 2,
    },
    {
      icon:
        "data:image/svg+xml;base64,PHN2ZyBpZD0iQ2FwYV8xIiBlbmFibGUtYmFja2dyb3VuZD0ibmV3IDAgMCA1MTIgNTEyIiBoZWlnaHQ9IjUxMiIgdmlld0JveD0iMCAwIDUxMiA1MTIiIHdpZHRoPSI1MTIiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGcgaWQ9IlhNTElEXzEzNTJfIj48ZyBpZD0iWE1MSURfMjUxXyI+PHBhdGggaWQ9IlhNTElEXzI2NV8iIGQ9Im00NDkuOTQyIDk5LjI2NmMwLTI3LjM2OS0yMi4yNjctNDkuNjM2LTQ5LjYzNi00OS42MzZoLTEyLjMwNmwtMzIuNzE1LTQ1LjQxM2MtLjAwMS0uMDAxLS4wMDItLjAwMi0uMDAyLS4wMDNsLS4wNDMtLjA1OWgtLjAwM2MtMS44NTItMi41NzEtNC44NTEtNC4xNTUtOC4xMTEtNC4xNTUgMCAwLTE4Mi4zNjcuMDExLTE4Mi42MzUuMDMyLTIuOTIzLjIzNi01LjU5NSAxLjc0My03LjMwOSA0LjEyM2wtMzIuNzU4IDQ1LjQ3NWgtMTIuNzI5Yy0yNy4zNyAwLTQ5LjYzNiAyMi4yNjctNDkuNjM2IDQ5LjYzNnY5NS40MDZjMCA1LjUyMyA0LjQ3NyAxMCAxMCAxMHMxMC00LjQ3NyAxMC0xMHYtOTUuNDA2YzAtMTYuMzQxIDEzLjI5NS0yOS42MzYgMjkuNjM2LTI5LjYzNmgxMy43MDhsMjkxLjA0NyAyOTEuMDQ3aC0zMzQuMzkydi03Ni4wMDVjMC01LjUyMy00LjQ3Ny0xMC0xMC0xMHMtMTAgNC40NzctMTAgMTB2MTgxLjMyM2MwIDI1LjM2NyAyMC42MzggNDYuMDA0IDQ2LjAwNCA0Ni4wMDRoMjk1Ljg3NWMyNS4zNjcgMCA0Ni4wMDQtMjAuNjM4IDQ2LjAwNC00Ni4wMDR2LTM2Ni43Mjl6bS0yMCAzMjUuNDExaC00OC4wNjZ2LTQ0aDQ4LjA2NnptMC0zMjUuNDExdjE2MS4yMzdsLTExNi44OTctMTE2Ljg5NyA3My45NzYtNzMuOTc2aDEzLjI4NWMxNi4zNDEgMCAyOS42MzYgMTMuMjk0IDI5LjYzNiAyOS42MzZ6bS02MC4xNDktNDAuNjkzLTcwLjg5MSA3MC44OS0yOC41NDgtMjguNTQ4IDc1LjUzMS03NS41M3ptLTQ2LjgwOS0zOC41NzMtNjYuNzcyIDY2Ljc3Mi02Ni43NzMtNjYuNzcyem0tMTU2LjQ0NiA1LjM4NSAyNjMuNDA0IDI2My40MDN2NTcuMDk3bC0yODcuMzEyLTI4Ny4zMTJ6bTE5NS4zMzggMzU1LjI5MnY0NGgtNTcuMjV2LTQ0em0tNzcuMjUxIDB2NDRoLTIwMi41Njd2LTQ0em0xMTkuMzEzIDExMS4zMjNoLTI5NS44NzVjLTE0LjMzOSAwLTI2LjAwNC0xMS42NjYtMjYuMDA0LTI2LjAwNHYtMjEuMzE4aDM0Ny44ODR2MjEuMzE4Yy0uMDAxIDE0LjMzOC0xMS42NjcgMjYuMDA0LTI2LjAwNSAyNi4wMDR6Ii8+PHBhdGggaWQ9IlhNTElEXzc2NF8iIGQ9Im03Mi4wNTggMjQ5LjY3YzIuNjMgMCA1LjIxLTEuMDcgNy4wNy0yLjkzczIuOTMtNC40MyAyLjkzLTcuMDdjMC0yLjYzLTEuMDctNS4yMS0yLjkzLTcuMDdzLTQuNDQtMi45My03LjA3LTIuOTMtNS4yMSAxLjA3LTcuMDcgMi45My0yLjkzIDQuNDQtMi45MyA3LjA3YzAgMi42NCAxLjA3IDUuMjEgMi45MyA3LjA3czQuNDQgMi45MyA3LjA3IDIuOTN6Ii8+PC9nPjwvZz48L3N2Zz4=",
      title: "Bathrobe",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 3,
    },
    {
      icon:
        "data:image/svg+xml;base64,PHN2ZyBpZD0iTGF5ZXJfMSIgZW5hYmxlLWJhY2tncm91bmQ9Im5ldyAwIDAgNTEyIDUxMiIgaGVpZ2h0PSI1MTIiIHZpZXdCb3g9IjAgMCA1MTIgNTEyIiB3aWR0aD0iNTEyIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPjxwYXRoIGQ9Im00MzAuOTc2IDI3NS4wODVjLTE3LjA1LTUuNjI0LTM2LjA4Mi0xMC4zMjgtNTYuNTM3LTE0LjA0OCAyNy44MTUtMTEuNjgxIDQ2LjA2Mi0yOC40MDMgNDYuMDYyLTQ5Ljk1MyAwLTMxLjAzLTM3LjgyNS01Mi4wNTYtODcuNTg3LTYyLjQyNCAxMS40NjUtMTAuMDQ2IDEzLjU4Ny0yMC42ODEgMTMuNTg3LTI3LjE2IDAtOC45MjItNC4wMTgtMjUuNzI1LTMwLjkyMi0zOC4wMTktMTYuMjAzLTcuNDAzLTM3LjM2Mi0xMS40ODEtNTkuNTc5LTExLjQ4MXMtNDMuMzc2IDQuMDc4LTU5LjU3OCAxMS40ODFjLTI2LjkwNCAxMi4yOTQtMzAuOTIyIDI5LjA5Ny0zMC45MjIgMzguMDE5IDAgNi40NzkgMi4xMjggMTcuMTEzIDEzLjU5MSAyNy4xNTktNDkuNzY0IDEwLjM2OC04Ny41OTEgMzEuMzk0LTg3LjU5MSA2Mi40MjUgMCAyMS41NSAxOC4yNDYgMzguMjczIDQ2LjA2IDQ5Ljk1NC0yMC40NTUgMy43MTktMzkuNDg3IDguNDIzLTU2LjUzNiAxNC4wNDctNjYuOTY3IDIyLjA5MS04MS4wMjQgNTAuNDg1LTgxLjAyNCA3MC40MTVzMTQuMDU3IDQ4LjMyNCA4MS4wMjQgNzAuNDE1YzQ3LjA4MiAxNS41MzEgMTA5LjIyNCAyNC4wODUgMTc0Ljk3NiAyNC4wODVzMTI3Ljg5NC04LjU1NCAxNzQuOTc2LTI0LjA4NWM2Ni45NjctMjIuMDkxIDgxLjAyNC01MC40ODUgODEuMDI0LTcwLjQxNXMtMTQuMDU3LTQ4LjMyNC04MS4wMjQtNzAuNDE1em0tMjIyLjA4NS0xNjQuMzE4YzEyLjE5My01LjU3MiAyOS4zNjQtOC43NjcgNDcuMTA5LTguNzY3czM0LjkxNiAzLjE5NSA0Ny4xMDkgOC43NjdjMTAuMDE5IDQuNTc4IDEzLjM5MSA5LjI4OCAxMy4zOTEgMTAuNzMzcy0zLjM3MiA2LjE1NS0xMy4zOTEgMTAuNzMzYy0xMi4xOTMgNS41NzItMjkuMzY0IDguNzY3LTQ3LjEwOSA4Ljc2N3MtMzQuOTE2LTMuMTk1LTQ3LjEwOS04Ljc2N2MtMTAuMDE5LTQuNTc4LTEzLjM5MS05LjI4OC0xMy4zOTEtMTAuNzMzczMuMzcyLTYuMTU1IDEzLjM5MS0xMC43MzN6bS01My4zNDcgMTI1LjAzN2MtMjMuMzkxLTguNTkyLTM0LjA0NC0xOC44MzctMzQuMDQ0LTI0LjcyczEwLjY1My0xNi4xMjkgMzQuMDQ0LTI0LjcyMWMyNi42NzYtOS43OTkgNjIuMzUzLTE1LjE5NiAxMDAuNDU2LTE1LjE5NnM3My43OCA1LjM5NiAxMDAuNDU2IDE1LjE5NmMyMy4zOTEgOC41OTIgMzQuMDQ0IDE4LjgzNyAzNC4wNDQgMjQuNzIxcy0xMC42NTMgMTYuMTI4LTM0LjA0NCAyNC43MmMtMjYuNjc3IDkuOC02Mi4zNTIgMTUuMTk2LTEwMC40NTYgMTUuMTk2cy03My43NzktNS4zOTYtMTAwLjQ1Ni0xNS4xOTZ6bTI2Ni4wMzQgMTUxLjYyMWMtNDQuMTMxIDE0LjU1OC0xMDIuOTM0IDIyLjU3NS0xNjUuNTc4IDIyLjU3NXMtMTIxLjQ0Ny04LjAxNy0xNjUuNTc4LTIyLjU3NWMtNDQuNTk4LTE0LjcxMi02MC40MjItMzEuNzc5LTYwLjQyMi00MS45MjVzMTUuODI0LTI3LjIxMyA2MC40MjItNDEuOTI1YzQ0LjEzMS0xNC41NTggMTAyLjkzNC0yMi41NzUgMTY1LjU3OC0yMi41NzVzMTIxLjQ0NyA4LjAxNyAxNjUuNTc4IDIyLjU3NWM0NC41OTggMTQuNzEyIDYwLjQyMiAzMS43NzkgNjAuNDIyIDQxLjkyNXMtMTUuODI0IDI3LjIxMy02MC40MjIgNDEuOTI1eiIvPjwvc3ZnPg==",
      title: "Hot Stones",
      content:
        "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.",
      id: 4,
    },
  ];
  const whatwedo = [
    {
      icon: "😊",
      title: "What we do One",
      content: "In Home Massages",
      id: 1,
    },
    {
      icon: "😊",
      title: "What we do Two",
      content: "Deep, Superficial Massages",
      id: 2,
    },

    {
      icon: "😊",
      title: "What we do Three",
      content: "In Home Massages",
      id: 3,
    },
    {
      icon: "😊",
      title: "What we do Four",
      content: " Outer Home Services",
      id: 4,
    },
    {
      icon: "😊",
      title: "What we do Four",
      content: "Santiosage",
      id: 5,
    },
    {
      icon: "😊",
      title: "What we do Four",
      content: " Reflexology",
      id: 6,
    },
    {
      icon: "😊",
      title: "What we do Four",
      content: "Nutritional Consultation",
      id: 7,
    },
    {
      icon: "😊",
      title: "What we do Four",
      content: "Personal Training",
      id: 8,
    },
    {
      icon: "😊",
      title: "What we do Four",
      content: "Volleyball Coaches ",
      id: 9,
    },
    {
      icon: "😊",
      title: "What we do Four",
      content: "Private Volleyball Lessons",
      id: 10,
    },
  ];
  import CTA from "../components/CTA.svelte";
  import Hero from "../components/Hero.svelte";
  let pageIntro =
    "Our mission is to promote relaxation, stress relief, and a pain free lifestyle though therapeutic massage and bodywork, while supporting you in healing yourself holistically.";
</script>

<svelte:head>
  <title>Home</title>
</svelte:head>

<Hero pageHeading="Welcome to Molten Massage International" {pageIntro} />
<div class="container whatwedo py-5 my-5">
  <h1 class="text-center py-3 section-header-text">What we do</h1>
  <h4 class="text-center mb-5" data-aos="fade-up" data-aos-delay="100">
    Molten Massage Int'l "Catering to your every PHYSICAL & PHYSIOLOGICAL needs"
    Specializing in:
  </h4>
  <div class="row" style="align-items:center">
    <div class="col-lg-6 col-md-12">
      <!-- svelte-ignore a11y-img-redundant-alt -->
      <img src="images/leg-massage.jpg" alt="Photo" class="img-fluid" />
    </div>
    <div class="col-lg-6 col-md-12">
      <div class="row ">
        {#each whatwedo as work}
          <div
            class="col-lg-6 mt-2 aos-init aos-animate"
            data-aos-delay="{work.id}00"
            data-aos="zoom-in"
          >
            <div class="card">
              <div class="card-body" style="display:flex; align-items:center;">
                <i class="icon-check mr-2" />
                <p class="card-text" style="margin-left:7px; font-size:0.90rem">
                  {work.content}
                </p>
              </div>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
</div>

<div class="container mission py-5 my-5">
  <h1 class="text-center py-3 mt-5 section-header-text">Mission Statement</h1>
  <div class="row" style="align-items:center">
    <div class="col-lg-6 col-md-12">
      <div class="row ">
        <div class="card">
          <div class="card-body">
            <p class="card-text mission-text">
              Our mission is to promote relaxation, stress relief, and a pain
              free lifestyle though therapeutic massage and bodywork, while
              supporting you in healing yourself holistically. MMI's focus is to
              provide natural solutions to you the client, as well as education
              that ultimately result in helping you realize optimal, physical
              and physiological health and happiness.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="col-lg-6 col-md-12">
      <!-- svelte-ignore a11y-img-redundant-alt -->
      <img src="images/mission.jpg" alt="Photo" class="img-fluid" />
    </div>
  </div>
</div>

<!-- Features -->
<CTA />
<div
  class="site-section bg-image overlay spa-features "
  style="background-image:url(../images/hero-bg.jpg); 
  background-attachment: fixed;
  padding:65px 0 ;margin-bottom:2rem;"
>
  <div class="container">
    <div class="row">
      <div class="col-12">
        <h2 class="text-white mb-5 section-header-text section-header-side">
          Massage Features
        </h2>
      </div>
    </div>
    <div class="row">
      {#each spa_features as spa}
        <div
          class="col-md-6 mb-4 col-sm-12 col-lg-3"
          data-aos="fade-up"
          data-aos-delay="{spa.id}00"
        >
          <div class="spa_block">
            <div class="wrap-icon">
              <span class="flaticon-towel" /><img
                src={spa.icon}
                alt=""
                class="img-fluid"
              />
            </div>
            <div class="text">
              <h3>{spa.title}</h3>
              <p>{spa.content}</p>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</div>
<!-- Testimonial -->
<div class="site-section py-5 my-5">
  <div class="text-center ">
    <h1 class="section-header-text text-black mb-2 text-center">
      Testimonials
    </h1>
  </div>
  <div class="container" id="carousel">
    <div class="nonloop-block-13 owl-carousel d-flex owl-loaded owl-drag">
      <div class="owl-stage-outer">
        <div
          class="owl-stage"
          style="transform: translate3d(-2898px, 0px, 0px); transition: all 1s ease 0s; width: 5313px;"
        >
          {#each testimonies as testimony}
            <div
              class="owl-item active card"
              style="width: 400px; margin-right: 20px;"
            >
              <div>
                <div class="testimonial-2">
                  <div class="d-flex v-card align-items-center mb-4">
                    <!-- svelte-ignore a11y-img-redundant-alt -->
                    <img
                      src={testimony.image}
                      alt="Image"
                      class="img-fluid mr-3"
                    />
                    <span>{testimony.name}</span>
                  </div>
                  <blockquote>
                    <p>"{testimony.content}"</p>
                  </blockquote>
                </div>
              </div>
            </div>
          {/each}
        </div>
      </div>
    </div>
  </div>
</div>

<!-- BIG QUOTE -->
<div class="site-section py-5 my-5">
  <div class="container">
    <div class="row align-items-center">
      <div class="col-md-5  mr-auto">
        <blockquote class="testimonial_38201">
          <p class=" h3  testimonial_38201">
            <span class="text-primary">“</span>Our mission is to promote
            relaxation, stress relief, and a pain free lifestyle though
            therapeutic massage and bodywork, while supporting you in healing
            yourself holistically..<span class="text-primary">”</span>
          </p>
          <p class="py-4">
            — Jean Doe,
            <span class="text-muted">Spa Customer</span>
          </p>
        </blockquote>
      </div>
      <div class="col-md-6">
        <div class="d-flex">
          <div
            class="bg-img-1 mr-md-4 mt-md-5"
            style="background-image:url(../images/testify-1.jpg)"
            data-aos="fade-up"
            data-aos-delay="100"
          />
          <div
            class="bg-img-1"
            style="background-image:url(../images/testify-2.jpg)"
            data-aos="fade-up"
            data-aos-delay="200"
          />
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  .whatwedo h4 {
    font-size: 20px;
  }
  .mission-text {
    line-height: 2;
    font-size: 20px;
    padding: 1.2rem 0;
  }
  .spa-features .spa_block {
    -webkit-transition: 0.3s all ease;
    -o-transition: 0.3s all ease;
    transition: 0.3s all ease;
    color: #fff;
    border-radius: 4px;
    background: #ffa1884d;
    /* background: #0000; */
  }
  .spa-features .spa_block h3 {
    color: #fff;
    font-size: 18px;
  }
  .spa-features .spa_block h3 {
    color: #fff;
    font-size: 18px;
  }
  .wrap-icon span {
    font-size: 2.4rem;
    color: #301c16;
  }
  .spa_block {
    padding: 30px;
    border: 1px solid #fff3;
  }
  .spa_block:hover {
    background-color: rgba(255, 255, 255, 0.288);
  }
  .testimonial-2 {
    background: #fff;
    padding: 30px;
    border-left: solid 5px #ffa188;
    border-radius: 5px;
    box-shadow: 0px 0px 30px rgb(157 161 175 / 15%);
    font-family: "Open Sans", sans-serif;
    line-height: 25px;
  }
  .testimonial-2 .v-card img {
    width: 50px;
    flex: 0 0 50px;
    border-radius: 50%;
  }
  .testimonial-2 blockquote {
    font-size: 1.3rem;
  }
  .testimonial_38201 p {
    line-height: 1.5;
    font-family: "Playfair Design";
  }
  #carousel {
    padding: 4rem 0;
    background-color: transparent;
  }
  .card {
    background: #ffa1884d;
  }
</style>
