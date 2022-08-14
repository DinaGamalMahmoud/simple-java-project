name: Build Java APP
on:
#   push:
#     branches:
#       - master
  workflow_dispatch:
      print_tags:
        description: 'True to print to STDOUT'
        required: true 
        type: boolean 
env:
  ACTIONS_ALLOW_UNSECURE_COMMANDS: true
jobs:
  build-java-app:
    name: Build Java APP
    runs-on: ubuntu-latest
#     if: github.ref == 'refs/heads/master'
    if:  ${{ inputs.print_tags }} 
    steps:
      - name: Print the input tag to STDOUT
        run: echo  The tags are ${{ inputs.tags }} 
#       - name: Checkout
#         uses: actions/checkout@v2
#         with:
#           fetch-depth: '0'

