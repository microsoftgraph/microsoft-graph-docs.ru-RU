---
title: Разрешение аппликатиосн на доступ к собраниям по сети от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям по сети от имени пользователя.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 8f0738d282cfe012b90293b067c87ab7dc284f9e
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843347"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a>Разрешение приложениям получать доступ к собраниям по сети от имени пользователя

В некоторых случаях, например, для фоновых служб или приложений-демонов, выполняемых на сервере без присутствия вошедшего пользователя, приложение может вызвать Microsoft Graph для выполнения действий от имени пользователя. Например, приложению может потребоваться вызвать Microsoft Graph, чтобы спланировать несколько собраний на основе опубликованных расписаний (таких как курсы) или внешних средств планирования. В таких случаях пользователь, работающий с приложением от имени, идентифицируется в качестве организатора собрания.

Администраторы, которые хотят разрешить приложению получать доступ к ресурсам собраний по сети от имени пользователя, могут использовать командлеты PowerShell **New-ксаппликатионакцессполици** и **Grant-ксаппликатионакцессполици** для настройки управления доступом. В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.

Эти действия относятся только к собраниям по сети и не распространяются на другие ресурсы Microsoft Graph.

## <a name="configure-application-access-policy"></a>Настройка политики доступа к приложениям

Чтобы настроить политику доступа к приложениям и разрешить приложениям получать доступ к собраниям по сети с разрешениями для приложений:

1. Определите апплкатион (Client) ID приложения и идентификаторы пользователей, от имени которых приложение будет авторизовано для доступа к собраниям по сети.

    - Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Определение идентификатора пользователя (объекта) пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)

2. Подключитесь к Skype для бизнеса PowerShell с помощью учетной записи админитратор. Дополнительные сведения: [Управление Skype для бизнеса Online с помощью PowerShell](https://docs.microsoft.com/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).

3. Создайте политику доступа к приложениям, содержащую список идентификаторов приложений.

    Выполните следующий командлет, заменив аргументы **Identity**, **AppID**и **Description** (необязательный параметр).

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. Предоставьте политике пользователю разрешение на доступ к собраниям по сети от имени предоставленного пользователя с помощью идентификаторов приложений, включенных в политику. 

   Выполните следующий командлет, заменив аргументы **PolicyName** и **Identity** .

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> **Примечание** 
> 
> - _Identity_ — это имя политики при создании политики, но идентификатор пользователя при предоставлении политики.
> - Для вступления в силу изменений в политиках доступа к приложениям в вызовах REST API Microsoft Graph может потребоваться до 30 минут.

## <a name="supported-permissions-and-additional-resources"></a>Поддерживаемые разрешения и дополнительные ресурсы

Администраторы могут использовать командлеты Аппликатионакцессполици для управления доступом к почтовым ящикам для приложения, которому предоставлено одно из следующих разрешений приложения:

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All

Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/new-csapplicationaccesspolicy).

## <a name="errors"></a>Ошибки

Если в вызове API отказано в доступе из-за того, что приложение пытается получить доступ к собранию по сети, когда политика доступа к приложениям не настроена, может возникнуть следующая ошибка.

```json
{
    "error": {
        "code": "Unauthorized",
        "message": "App <app_ID_redacted> is not authorized to Create meeting on behalf of user <user_ID_redacted>",
        "innerError": {
            "date": "<date_redacted>",
            "request-id": "599d9cb0-56ac-4dc5-b6f8-1456a1414609"
        }
    }
}
```

Выполните действия, описанные в этой статье, чтобы создать и/или предоставить политику доступа к приложению, содержащую идентификатор приложения, в идентификатор пользователя.

## <a name="see-also"></a>См. также

- [Справочник по разрешениям](permissions-reference.md)
- [New-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/new-csapplicationaccesspolicy)
- [Granting — Аппликатионакцессполици](https://docs.microsoft.com/powershell/module/skype/grant-csapplicationaccesspolicy)
- [Get-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/get-csapplicationaccesspolicy)
- [Set-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/set-csapplicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/remove-csapplicationaccesspolicy)
