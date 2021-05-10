---
title: Ограничение области разрешений для приложений с указанием определенных почтовых ящиков Exchange Online
description: Чтобы ограничить область разрешений для приложений с указанием определенных почтовых ящиков Exchange Online, потребуется создать политики доступа приложений.
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: f31f7bfc8ff72c8f3cb9e6f61185187f50bab7fc
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266838"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a>Ограничение области разрешений для приложений с указанием определенных почтовых ящиков Exchange Online 

Некоторые приложения вызывают Microsoft Graph от своего имени, а не от имени пользователя. Обычно это фоновые службы и управляющие программы, которые работают на сервере без выполнившего вход пользователя. В таких приложениях используется [поток предоставления учетных данных клиента OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow), обеспечивающий проверку подлинности, и заданы настройки разрешений для приложений, которые позволяют таким приложениям получать доступ ко всем почтовым ящикам организации на сервере Exchange Online. Например с помощью разрешения для приложения Mail.Read приложения могут считывать почту во всех почтовых ящиках без выполнившего вход пользователя. 

Администраторам, которые хотят ограничить доступ приложения к определенному набору почтовых ящиков, можно воспользоваться командлетом PowerShell **New-ApplicationAccessPolicy**, чтобы настроить управление доступом. В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.

Эти инструкции относятся к ресурсам Exchange Online и не относятся к другим рабочим нагрузкам Microsoft Graph. 

## <a name="configure-applicationaccesspolicy"></a>Настройка ApplicationAccessPolicy

Чтобы настроить политику доступа приложения и ограничить область разрешений для приложения, выполните указанные ниже действия.
1.  Подключитесь к Exchange Online PowerShell. Подробнее см. статью [Подключение к Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).

2.  Определите идентификатор клиента приложения и группу безопасности с поддержкой электронной почты, чтобы ограничить доступ приложения.

    - Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Создайте новую группу безопасности с поддержкой электронной почты или используйте существующую и определите адрес электронной почты для группы. 

3.  Создайте политику доступа приложения. 

    Выполните указанную ниже команду, заменив аргументы **AppId**, **PolicyScopeGroupId** и **Description**.
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  Протестируйте созданную политику доступа приложения.

    Выполните указанную ниже команду, заменив аргументы **AppId** и **Identity**.
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    В результате выполнения этой команды будет указано, имеет ли приложение доступ к почтовому ящику пользователя User1.

>**Примечание. Чтобы изменения политик доступа приложения вступили в силу в вызовах API Microsoft Graph REST, может потребоваться до 30 минут.**

## <a name="supported-permissions-and-additional-resources"></a>Поддерживаемые разрешения и дополнительные ресурсы
Администраторы могут использовать командлеты ApplicationAccessPolicy для управления доступом к почтовым ящикам приложения, которому предоставлены указанные ниже разрешения. 
- Mail.Read
- Mail.ReadBasic
- Mail.ReadBasic.All
- Mail.ReadWrite
- Mail.Send
- MailboxSettings.Read  
- MailboxSettings.ReadWrite
- Calendars.Read
- Calendars.ReadWrite
- Contacts.Read
- Contacts.ReadWrite

Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy). 

## <a name="handling-api-errors"></a>Обработка ошибок API
Если API-вызову будет отказано в доступе из-за настроек политики доступа приложения, может появиться указанное ниже сообщение об ошибке. 
```json
{
    "error": {
        "code": "ErrorAccessDenied",
        "message": "Access to OData is disabled.",
        "innerError": {
            "request-id": "2f038156-cf40-403d-8e46-831fe42a8229",
            "date": "2019-05-24T10:16:21"
        }
    }
}
```
Если по API-вызовам Microsoft Graph из вашего приложения отображается такое сообщение об ошибке, обратитесь к администратору Exchange Online организации, чтобы убедиться в том, что у вашего приложения есть разрешение на доступ к ресурсу почтового ящика.



## <a name="see-also"></a>Дополнительные ресурсы

- [Справочник по разрешениям](permissions-reference.md)
- [New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [Get-ApplicationAccessPolicy](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [Set-ApplicationAccessPolicy](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [Test-ApplicationAccessPolicy](/powershell/module/exchange/organization/test-applicationaccesspolicy)
