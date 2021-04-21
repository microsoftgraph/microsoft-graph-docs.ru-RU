---
title: Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям в Интернете от имени пользователя.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: ff14ae4506cc19adf58ab61cde436a0252bd6f5c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920399"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a>Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя

В некоторых случаях, например в фоновых службах или приложениях daemon, которые работают на сервере без присутствия подписанного пользователя, приложение может вызвать Microsoft Graph для действий от имени пользователя. Например, приложению может потребоваться вызвать Microsoft Graph, чтобы запланировать несколько собраний на основе опубликованных расписания (например, курсов) или внешних средств планирования. В этих случаях пользователь, который действует от имени приложения, определен как организатор собрания.

Администраторы, которые хотят разрешить приложению доступ к ресурсам собраний в Интернете от имени пользователя, могут использовать команды **New-CsApplicationAccessPolicy** и **Grant-CsApplicationAccessPolicy** PowerShell для настройки управления доступом. В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.

Эти действия относятся к собраниям в Интернете и не применяются к другим ресурсам Microsoft Graph.

## <a name="configure-application-access-policy"></a>Настройка политики доступа к приложениям

Чтобы настроить политику доступа к приложениям и разрешить приложениям получать доступ к собраниям в Интернете с разрешениями приложений:

1. Определите ID приложения (клиента) и пользовательские ИД пользователей, от имени которых приложение будет уполномочено получать доступ к собраниям в Интернете.

    - Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Идентификация пользователя (объекта) на портале управления пользователями [Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)

2. Подключение к Skype для бизнеса PowerShell с учетной записью администратора. Подробные сведения см. [в материале Управление Skype для бизнеса Online с помощью PowerShell.](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)

3. Создайте политику доступа к приложениям, содержащую список ID приложений.

    Запустите следующий cmdlet, заменив **аргументы Identity,** **AppIds** и **Description** (необязательный).

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. Предоставление политики пользователю, чтобы позволить ID-данным приложения, содержающимся в политике, получать доступ к собраниям в Интернете от имени предоставленного пользователя. 

   Запустите следующий комдлет, заменив **аргументы PolicyName** и **Identity.**

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> [!NOTE]
> - _Identity_ ссылается на имя политики при создании политики, но идентификатор пользователя при предоставлении политики.
> - Изменение политик доступа к приложениям может занять до 30 минут, чтобы внести изменения в API API MICROSOFT Graph REST.

## <a name="supported-permissions-and-additional-resources"></a>Поддерживаемые разрешения и дополнительные ресурсы

Администраторы могут использовать cmdlets ApplicationAccessPolicy для управления доступом к почтовым ящикам для приложения, которое было предоставлено любое из следующих разрешений приложения:

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All

Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).

## <a name="errors"></a>Ошибки

Вы можете столкнуться со следующей ошибкой, когда вызову API отказано в доступе из-за того, что приложение пытается получить доступ к собранию в Интернете, если политика доступа к приложениям не настроена.

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

Следуйте шагам в этой статье, чтобы создать и/или предоставить политику доступа к приложениям, которая содержит ID приложения для пользовательского ИД.

## <a name="see-also"></a>См. также

- [Справочник по разрешениям](permissions-reference.md)
- [New-CsApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy)
- [Grant-CsApplicationAccessPolicy](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [Get-CsApplicationAccessPolicy](/powershell/module/skype/get-csapplicationaccesspolicy)
- [Set-CsApplicationAccessPolicy](/powershell/module/skype/set-csapplicationaccesspolicy)
- [Remove-CsApplicationAccessPolicy](/powershell/module/skype/remove-csapplicationaccesspolicy)
