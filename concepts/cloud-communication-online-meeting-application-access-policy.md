---
title: Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя
description: Узнайте, как настроить приложения для доступа к собраниям в Интернете от имени пользователя.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 6856e35fa9bad4f220b10e5a8c945f91ae4a2ff6a43c65ed5fe7af34ce69ded5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235179"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a>Разрешить приложениям получать доступ к собраниям в Интернете от имени пользователя

В некоторых случаях, например в фоновых службах или приложениях daemon, которые работают на сервере без присутствия подписанного пользователя, приложение может вызвать microsoft Graph, чтобы принять меры от имени пользователя. Например, приложению может потребоваться вызвать microsoft Graph, чтобы запланировать несколько собраний, основанных на опубликованных расписаниях (например, курсах) или внешних средствах планирования. В этих случаях пользователь, который действует от имени приложения, определен как организатор собрания.

Администраторы, которые хотят разрешить приложению доступ к ресурсам собраний в Интернете от имени пользователя, могут использовать команды **New-CsApplicationAccessPolicy** и **Grant-CsApplicationAccessPolicy** PowerShell для настройки управления доступом. В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения.

Эти действия относятся к собраниям в Интернете и не применяются к другим Graph Майкрософт.

## <a name="configure-application-access-policy"></a>Настройка политики доступа к приложениям

Чтобы настроить политику доступа к приложениям и разрешить приложениям получать доступ к собраниям в Интернете с разрешениями приложений:

1. Определите ID приложения (клиента) и пользовательские ИД пользователей, от имени которых приложение будет уполномочено получать доступ к собраниям в Интернете.

    - Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Идентификация пользователя (объекта) на портале управления пользователями [Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)

2. Подключение Skype для бизнеса PowerShell с учетной записью администратора. Подробные сведения см. в [Skype для бизнеса Управление Skype для бизнеса с PowerShell.](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)

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
5. (Необязательный) Предоставление политики для всего клиента. Это применимо к пользователям, которым не назначена политика доступа к приложениям. Подробные сведения см. в разделе [](#see-also) ссылки на раздел cmdlet.

   Запустите следующий комдлет, заменив аргумент **PolicyName.**

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Global
   ```

> [!NOTE]
> - _Identity_ ссылается на имя политики при создании политики, но идентификатор пользователя при предоставлении политики.
> - Изменение политик доступа к приложениям может занять до 30 минут для звонков microsoft Graph API REST.

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
