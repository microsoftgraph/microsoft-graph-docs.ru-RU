---
title: Ограничение разрешений для приложений с указанием определенных почтовых ящиков Exchange Online
description: Чтобы ограничить область разрешений для приложений с указанием определенных почтовых ящиков Exchange Online, потребуется создать политики доступа приложений.
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: 54f899f9a4b1f7fba71acaa476f994b742ad58a6cfa3cc51d18adb42ee1a3c50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141219"
---
# <a name="limiting-application-permissions-to-specific-exchange-online-mailboxes"></a>Ограничение разрешений для приложений с указанием определенных почтовых ящиков Exchange Online 

Администраторы, которые хотят ограничить доступ приложения определенными почтовыми ящиками, могут создать политику доступа приложений с помощью командлета PowerShell **New-ApplicationAccessPolicy**. В этой статье описаны основные действия по настройке управления доступом. Эти инструкции относятся к ресурсам Exchange Online и не относятся к другим рабочим нагрузкам Microsoft Graph. 

## <a name="background"></a>Общие сведения
Некоторые приложения вызывают Microsoft Graph от своего имени, а не от имени пользователя. Обычно это фоновые службы и управляющие программы, которые работают на сервере без выполнившего вход пользователя. В таких приложениях используется [поток предоставления учетных данных клиента OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow), обеспечивающий проверку подлинности, и заданы настройки разрешений для приложений, которые по умолчанию позволяют таким приложениям получать доступ ко _всем_ почтовым ящикам организации в Exchange Online. Например с помощью разрешения для приложения `Mail.Read` приложения могут считывать почту во всех почтовых ящиках без необходимости входа пользователя. 

Существуют сценарии, в которых администраторам может потребоваться разрешить приложению доступ только к определенным почтовым ящикам, а _не ко всем_ почтовым ящикам Exchange Online в организации. Администраторы могут определить набор почтовых ящиков для разрешения доступа, поместив их в группу безопасности с поддержкой почты. Затем администраторы могут ограничить доступ сторонних приложений только этим набором почтовых ящиков, создав политику доступа приложений для доступа к этой группе.

> [!NOTE]
> После настройки политики доступа приложений для организации эта политика применяется ко всем приложениям, использующим API Microsoft Graph или веб-службы Exchange для доступа к почтовым ящикам Exchange Online.

Как описано далее в разделе [Поддерживаемые разрешения и дополнительные ресурсы](#supported-permissions-and-additional-resources), политика доступа приложений ограничивает доступ к почтовым ящикам только приложениями, которым были предоставлены любые разрешения Microsoft Graph или веб-служб Exchange, поддерживаемые политикой.

## <a name="configure-applicationaccesspolicy"></a>Настройка ApplicationAccessPolicy

Чтобы настроить политику доступа приложения и ограничить область разрешений для приложения, выполните указанные ниже действия.
1.  Подключитесь к Exchange Online PowerShell. Подробнее см. статью [Подключение к Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).

2.  Определите идентификатор клиента приложения и группу безопасности с поддержкой электронной почты, чтобы ограничить доступ приложения.

    - Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Создайте новую группу безопасности с поддержкой электронной почты или используйте существующую и определите адрес электронной почты для группы. 

3.  Создайте политику доступа приложения. 

    Выполните указанную ниже команду, заменив аргументы **AppId**, **PolicyScopeGroupId** и **Description**.
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  Протестируйте созданную политику доступа приложений.

    Выполните указанную ниже команду, заменив аргументы **Identity** и **AppId**.
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    В результате выполнения этой команды будет указано, имеет ли приложение доступ к почтовому ящику пользователя User1.

>**Примечание. Чтобы изменения политик доступа приложения вступили в силу в вызовах API Microsoft Graph REST, может потребоваться до 30 минут.**

## <a name="supported-permissions-and-additional-resources"></a>Поддерживаемые разрешения и дополнительные ресурсы

Администраторы могут использовать командлеты ApplicationAccessPolicy для управления доступом к почтовым ящикам для приложения, которому предоставлены указанные ниже разрешения приложений Microsoft Graph или разрешения веб-служб Exchange. 

Разрешения приложений Microsoft Graph: 
- `Mail.Read`
- `Mail.ReadBasic`
- `Mail.ReadBasic.All`
- `Mail.ReadWrite`
- `Mail.Send`
- `MailboxSettings.Read`
- `MailboxSettings.ReadWrite`
- `Calendars.Read`
- `Calendars.ReadWrite`
- `Contacts.Read`
- `Contacts.ReadWrite`

Область разрешений веб-служб Exchange: `full_access_as_app`.

Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/exchange/new-applicationaccesspolicy?view=exchange-ps&preserve-view=true). 


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
Если вызовы API Microsoft Graph из вашего приложения возвращают такое сообщение об ошибке, обратитесь к администратору Exchange Online организации, чтобы убедиться в наличии у вашего приложения разрешения на доступ к ресурсу почтового ящика.



## <a name="see-also"></a>См. также

- [Справочник по разрешениям](permissions-reference.md)
- [New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [Get-ApplicationAccessPolicy](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [Set-ApplicationAccessPolicy](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [Test-ApplicationAccessPolicy](/powershell/module/exchange/organization/test-applicationaccesspolicy)
- [Поддержка политики доступа приложений в EWS](https://techcommunity.microsoft.com/t5/exchange-team-blog/application-access-policy-support-in-ews/ba-p/2110361)
