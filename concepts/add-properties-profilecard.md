---
title: Настройка карточки профиля с помощью API профиля в Microsoft Graph (предварительная версия)
description: В этой статье описано, как настроить карточку профиля, сделав видимыми дополнительные атрибуты или добавив настраиваемые атрибуты.
author: PollyNincevic
localization\_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 85ec4c8bd842b01f441ef6c34b2c7be288ec059d5a30f3d73ac796cdc64e76be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146336"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a>Добавление свойств в карточку профиля с помощью API карточки профиля в Microsoft Graph (предварительная версия)

На [карточке профиля](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) в Microsoft 365 находится информация о пользователях, сохраненная и управляемая вашей организацией, например **Должность** или **Местонахождение офиса**.

Используйте ресурс [profileCardProperty](/graph/api/resources/profilecardproperty), чтобы отображать дополнительные свойства из Azure AD в карточках профилей для организации следующим образом:

* Обеспечение видимости дополнительных атрибутов
* Добавление настраиваемых атрибутов

Дополнительные свойства отображаются в разделе **Контакт** карточки профиля в Microsoft 365.

> [!NOTE]
> Операции на **ресурсе profileCardProperty** с использованием делегирования разрешений требуют от пользователя, вписаного, роли администратора клиента или глобального администратора.

## <a name="make-additional-attributes-visible"></a>Обеспечение видимости дополнительных атрибутов

Вы можете сделать видимыми в карточках профилей пользователей следующие атрибуты из Azure Active Directory (Azure AD). В этих атрибутах *регистр не учитывается*:

* `UserPrincipalName`
* `Fax`
* `StreetAddress`
* `PostalCode`
* `StateOrProvince`
* `Alias`

В таблице ниже показано соответствие атрибутов Azure AD свойствам объекта [user](/graph/api/resources/user) Microsoft Graph.

| Атрибут Azure AD | Свойство объекта user |
| ------------------ | -------------------- |
| UserPrincipalName | userPrincipalName |
| Fax | faxNumber |
| StreetAddress | streetAddress |
| PostalCode | postalCode |
| StateOrProvince | state |
| Alias | mailNickname |

Любой из этих атрибутов можно добавить в карточку профиля, настроив параметры организации и добавив атрибут в качестве свойства **directoryPropertyName** **профиляCardProperty** в Microsoft Graph. [](/graph/api/resources/organizationsettings) Когда вы делаете дополнительные атрибуты видимыми, вы должны использовать имена свойств в формате `en-us`. Вам не требуется добавлять локализованные значения. Дополнительные свойства будут автоматически отображаться с использованием языковых настроек, указанных пользователем в Microsoft 365.

> [!IMPORTANT]
> При добавлении атрибута в карточку профиля его отображение занимает до 24 часов.

### <a name="example"></a>Пример

В следующем примере атрибут `Alias` отображается на карточке профиля.

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

При успешном выполнении возвращается код отклика `201 OK` и объект **profileCardProperty** в тексте отклика. Значение `Alias` атрибута будет отображаться на карточке профиля пользователя.

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a>Добавление настраиваемых атрибутов

Вы можете добавлять в карточки профилей пользователей любой из 15 [настраиваемых атрибутов расширений](/graph/api/resources/onpremisesextensionattributes) Azure AD путем настройки параметров организации и [добавления соответствующего значения в качестве profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties) в Microsoft Graph. Вы можете добавить один ресурс **profileCardProperty** за один раз.

Отображение внесенных изменений в карточках профилей занимают до 24 часов.

Настраиваемые свойства не поддерживают поиск, и их невозможно использовать для поиска людей в различных приложениях и службах Майкрософт.

В таблице ниже показано, как имена настраиваемых атрибутов расширений Azure AD соответствуют поддерживаемым значениям свойства **directoryPropertyName** ресурса [profileCardProperty](/graph/api/resources/profilecardproperty). В именах настраиваемых атрибутов расширений Azure AD *регистр не учитывается*:

| Настраиваемый атрибут расширения Azure AD | Значение, указываемое в качестве directoryPropertyName |
| ----------------------------------- | ----------------------------------------- |
| extensionAttribute1 | customAttribute1 |
| extensionAttribute2 | customAttribute2 |
| extensionAttribute3 | customAttribute3 |
| extensionAttribute4 | customAttribute4 |
| extensionAttribute5 | customAttribute5 |
| extensionAttribute6 | customAttribute6 |
| extensionAttribute7 | customAttribute7 |
| extensionAttribute8 | customAttribute8 |
| extensionAttribute9 | customAttribute9 |
| extensionAttribute10 | customAttribute10 |
| extensionAttribute11 | customAttribute11 |
| extensionAttribute12 | customAttribute12 |
| extensionAttribute13 | customAttribute13 |
| extensionAttribute14 | customAttribute14 |
| extensionAttribute15 | customAttribute15 |

### <a name="example"></a>Пример

В следующем примере в карточку профиля добавляется первый настраиваемый атрибут расширения Azure AD, используемый для отображения имени **Cost center**. Для пользователей, выбравших в языковых настройках немецкий язык, отображаемым именем будет **Kostenstelle**.

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

Если язык не поддерживается, имя свойства отображается с использованием значения по умолчанию.

При успешном выполнении возвращается код отклика `201 OK` и объект **profileCardProperty** в тексте отклика. В этом примере вы можете предположить, что в карточке профиля отображается **Kostenstelle** для всех пользователей, выбравших в языковых настройках немецкий язык. Для всех остальных пользователей в карточке профиля отображается **Cost center**.

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "customAttribute1",
  "annotations": [
    {
      "displayName": "Cost center",
      "localizations": [
        {
          "languageTag": "de",
          "displayName": "Kostenstelle"
        }
      ]
    }
  ]
}
```

## <a name="see-also"></a>См. также

- [Поиск идентификатора клиента Microsoft 365](/onedrive/find-your-office-365-tenant-id)
- [Тип ресурса onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes)
- [Тип ресурса user](/graph/api/resources/user)
- [Песочница Graph](https://developer.microsoft.com/graph/graph-explorer)
- [Получение ресурса profileCardProperty](/graph/api/profilecardproperty-get)
