Для корректной работы с snr нужн одописать в файле /home/ans/.ansible/collections/ansible_collections/cisco/ios/plugins/terminal/ios.py

В функции get_privilege_level
перед строкой  prompt = self.privilege_revel_re.search(result)

"if result == 'Current privilege level is network-admin':
            result = 'Current privilege level is 15'"
