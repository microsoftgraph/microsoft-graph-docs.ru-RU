---
title: Разрешение приложениям доступа к собраниям по сети от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям по сети от имени пользователя.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 46a91349a6a19b0caab62c6ea9712a3b5d798ac3
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239291"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a>Разрешение приложениям доступа к собраниям по сети от имени пользователя

В некоторых случаях, например фоновых службах или приложениях-программах, которые работают на сервере без необходимости вличия пользователя, приложение может вызвать Microsoft Graph, чтобы выполнить действия от имени пользователя. Например, приложению может потребоваться вызвать Microsoft Graph для планирования нескольких собраний на основе опубликованных расписаний (например, курсов) или внешних средств планирования. В таких случаях пользователь, от имени пользователя, от имени пользователя, будет определен как организатор собрания.

Администраторы, которые хотят разрешить приложению доступ к ресурсам собраний по сети от имени пользователя, могут использовать для настройки управления доступом **new-CsApplicationAccessPolicy** и **Grant-CsApplicationAccessPolicy** PowerShell. В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.

Эти действия относятся к собраниям по сети и не применимы к другим ресурсам Microsoft Graph.

## <a name="configure-application-access-policy"></a>Настройка политики доступа к приложениям

Чтобы настроить политику доступа к приложениям и разрешить приложениям доступ к собраниям по сети с разрешениями для приложений:

1. Определите applcation (client) ID приложения и ИД пользователей, от имени которых приложение будет иметь право на доступ к собраниям по сети.

    - Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Идентификация пользовательского (объектного) ИД на портале [управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)

2. Подключите к Skype для бизнеса PowerShell с помощью учетной записи администратора. Подробные сведения см. в под [управлением Skype для бизнеса Online с помощью PowerShell.](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)

3. Создайте политику доступа к приложениям, содержащую список ИД приложения.

    Запустите следующий cmdlet, заменив **аргументы Identity,** **AppIds** и **Description** (необязательно).

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. Предоставить пользователю политику, чтобы разрешить содержающимся в ней ИД приложения доступ к собраниям по сети от имени предоставленного пользователя. 

   Запустите следующий cmdlet, заменив **аргументы PolicyName** и **Identity.**

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> **Примечание** 
> 
> - _Идентификатор_ ссылается на имя политики при создании политики, но идентификатор пользователя при ее предоставлении.
> - Изменение политик доступа к приложениям может занять до 30 минут, чтобы внести изменения в вызовы REST API Microsoft Graph.

## <a name="supported-permissions-and-additional-resources"></a>Поддерживаемые разрешения и дополнительные ресурсы

Администраторы могут использовать cmdlets ApplicationAccessPolicy для управления доступом к почтовым ящикам для приложения, которое имеет любое из следующих разрешений приложения:

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All

Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).

## <a name="errors"></a>Ошибки

Если вызову API отказано в доступе из-за того, что приложение пытается получить доступ к собранию по сети, если политика доступа к приложению не настроена, может возникнуть следующая ошибка.

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

Следуйте шагам в этой статье, чтобы создать и/или предоставить политику доступа к приложениям, которая содержит ИД приложения для ИД пользователя.

## <a name="see-also"></a>См. также

- [Справочник по разрешениям](permissions-reference.md)
- [New-CsApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy)
- [Grant-CsApplicationAccessPolicy](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [Get-CsApplicationAccessPolicy](/powershell/module/skype/get-csapplicationaccesspolicy)
- [Set-CsApplicationAccessPolicy](/powershell/module/skype/set-csapplicationaccesspolicy)
- [Remove-CsApplicationAccessPolicy](/powershell/module/skype/remove-csapplicationaccesspolicy)
