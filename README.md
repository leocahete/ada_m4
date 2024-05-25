# Princípios SOLID
- Single Responsibility (Caso 1)
    - Responsabilidade única de configuração dos filtros de segurança aplicados aos endpoints
    - Package: br.gov.caixa.banco.security
    - Classe: WebSecurityConfig
    - Linhas: 28 a 45
- Single Responsibility (Caso 2)
    - Responsabilidade única de tratamento de um token padrão JWT
    - Package: br.gov.caixa.banco.login
    - Classe: JWTService
    - Linhas: Classe como um todo
- Liskov Substitution:
    - Possibilidade de uso da classe mãe no lugar da classe filha
    - Package: br.gov.caixa.banco.service.transferencia
    - Classe: ContaCorrentePFService
    - Linhas: 54, 66, 75, 81, 87, 92, 101
- Interface Segregation (Caso 1):
    - Segregação das interfaces conforme particularidades dos clientes PF e PJ 
    - Package: br.gov.caixa.banco.service.saque
    - Classes: Saque, SaquePFImpl e SaquePJImpl
    - Linhas: As interfaces como um todo
- Interface Segregation (Caso 2):
    - Segregação das interfaces conforme particularidades dos clientes PF e PJ 
    - Package: br.gov.caixa.banco.service.transferencia
    - Classes: Transferencia, TransferenciaPFImpl e TransferenciaPJImpl
    - Linhas: As interfaces como um todo
    
# Design Patterns
- Chain Of Responsibility
    - Padrão: Comportamental
    - Package: br.gov.caixa.banco.exception
    - Classe: GlobalExceptionHandler
    - Linhas: Todos os métodos anotados com @ExceptionHandler
- Builder
    - Padrão: Criacional
    - Package: br.gov.caixa.banco.usuario
    - Classe: Usuario
    - Linhas: 41 e 42 
    
OBS: Infelizmente o tempo acabou, professor... São 23:30

Lamento por não conseguir buildar o código e nem implementar no código os princípios SOLID e os patterns
