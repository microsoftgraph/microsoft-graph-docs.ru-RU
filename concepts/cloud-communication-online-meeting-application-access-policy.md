---
title: Настройка политики доступа к приложениям с помощью API облачных коммуникаций
description: Используйте API облачных коммуникаций в Microsoft Graph, чтобы настроить политику доступа, которая позволяет приложениям получать доступ к собраниям по сети от имени пользователя.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 89015fffb8713f00f7d54d9eaa8e43272d03ca45
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436356"
---
# <a name="configure-application-access-to-online-meetings"></a>Настройка доступа приложений к собраниям по сети

API облачных коммуникаций в Microsoft Graph можно использовать для настройки политики доступа к приложениям, которая позволяет приложениям получать доступ к собраниям по сети от имени пользователя.

В некоторых случаях, например для фоновых служб или управляющих приложений, которые выполняются на сервере без присутствия вошедвшего пользователя, приложение может вызывать Microsoft Graph для выполнения действий от имени пользователя. Например, приложению может потребоваться вызвать Microsoft Graph, чтобы запланировать несколько собраний на основе опубликованных расписаний (например, курсов) или внешних средств планирования. В таких случаях пользователь, от имени которого выполняется приложение, определяется как организатор собрания.

Администраторы, которые хотят разрешить приложению доступ к ресурсам собраний по сети от имени пользователя, могут использовать командлеты **PowerShell New-CsApplicationAccessPolicy** и **Grant-CsApplicationAccessPolicy** PowerShell.

В этой статье описаны основные действия, которые необходимо выполнить для настройки политики доступа приложения. Эти действия относятся к собраниям по сети и не применяются к другим ресурсам Microsoft Graph.

## <a name="configure-application-access-policy"></a>Настройка политики доступа к приложениям

Чтобы настроить политику доступа к приложениям и разрешить приложениям доступ к собраниям по сети с разрешениями приложения, выполните указанные ниже действия.

1. Определите идентификатор приложения (клиента) и идентификаторы пользователей, от имени которых приложение будет иметь право на доступ к собраниям по сети.

    - Определите идентификатор приложения (клиента) на [портале регистрации приложений Azure](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).
    - Определение идентификатора пользователя (объекта) на портале [управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)

2. Подключитесь к Skype для бизнеса PowerShell с помощью учетной записи администратора. Дополнительные сведения см. в Skype для бизнеса [Online с помощью PowerShell](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell).

3. Создайте политику доступа к приложениям, содержащую список идентификаторов приложений.

    Выполните следующий командлет, заменив аргументы **Identity**, **AppIds** и **Description** (необязательно).

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. Предоставьте пользователю политику, чтобы разрешить идентификаторам приложений, содержащимся в политике, доступ к собраниям по сети от имени предоставленного пользователя. 

   Выполните следующий командлет, заменив **аргументы PolicyName** и **Identity** .

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "748d2cbb-3b55-40ed-8c34-2eae5932b22a"
   ```
5. (Необязательно) Предоставьте политику всему клиенту. Это применимо к пользователям, которым не назначена политика доступа к приложениям. Дополнительные сведения см. по ссылкам на командлеты в [разделе также](#see-also) .

   Выполните следующий командлет, заменив **аргумент PolicyName** .

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Global
   ```

> [!NOTE]
> - _Удостоверение_ ссылается на имя политики при создании политики, но идентификатор пользователя при предоставлении политики.
> - Изменения политик доступа к приложениям могут внести в вызовы REST API Microsoft Graph до 30 минут.

## <a name="supported-permissions-and-additional-resources"></a>Поддерживаемые разрешения и дополнительные ресурсы

Администраторы могут использовать командлеты ApplicationAccessPolicy для управления доступом к собраниям по сети для приложения, которое имеет любое из следующих разрешений приложения:

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All
- OnlineMeetingArtifact.Read.All

Дополнительные сведения о настройке политики доступа приложения см. в справочнике по командлету PowerShell [New-ApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy).

## <a name="errors"></a>Ошибки

При отказе в доступе к вызову API из-за того, что приложение пытается получить доступ к собранию по сети, если политика доступа к приложению не настроена, может возникнуть следующую ошибку.

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

Выполните действия, описанные в этой статье, чтобы создать и (или) предоставить политику доступа к приложениям, содержащую идентификатор приложения для идентификатора пользователя.

## <a name="see-also"></a>См. также

- [Справочник по разрешениям](permissions-reference.md)
- [New-CsApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy)
- [Grant-CsApplicationAccessPolicy](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [Get-CsApplicationAccessPolicy](/powershell/module/skype/get-csapplicationaccesspolicy)
- [Set-CsApplicationAccessPolicy](/powershell/module/skype/set-csapplicationaccesspolicy)
- [Remove-CsApplicationAccessPolicy](/powershell/module/skype/remove-csapplicationaccesspolicy)
- [Общие сведения об API облачных коммуникаций](cloud-communications-concept-overview.md)
