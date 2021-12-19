---
title: Добавление или удаление настраиваемых свойств на карточке профиля с помощью API карточки профиля в Microsoft Graph (предварительная версия)
description: Как настроить карточку профиля, сделав видимыми дополнительные атрибуты или добавив настраиваемые атрибуты. Вы также можете удалить настраиваемые атрибуты.
author: PollyNincevic
ms.localizationpriority: high
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 5e1b140f5e3c9612475bcf0a6e404168cced1c92
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61561512"
---
# <a name="add-or-delete-custom-properties-from-the-profile-card-using-the-profile-card-api-in-microsoft-graph-preview"></a>Добавление или удаление настраиваемых свойств на карточке профиля с помощью API карточки профиля в Microsoft Graph (предварительная версия)

На [карточке профиля](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) в Microsoft 365 находится информация о пользователях, сохраненная и управляемая вашей организацией, например **Должность** или **Местонахождение офиса**.

Используйте ресурс [profileCardProperty](/graph/api/resources/profilecardproperty), чтобы отображать дополнительные свойства из Azure AD в карточках профилей для организации следующим образом:

* Обеспечение видимости дополнительных атрибутов
* Добавление настраиваемых атрибутов

Дополнительные свойства отображаются в разделе **Контакт** карточки профиля в Microsoft 365.

Вы также можете [удалить](/graph/api/profilecardproperty-delete?view=graph-rest-beta&preserve-view=true) настраиваемые атрибуты из карточек профилей организации.

> [!NOTE]
> Операции в ресурсе **profileCardProperty**, использующем делегированные разрешения, требуют, чтобы у вошедшего пользователя была роль администратора клиента или глобального администратора.

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

Вы можете добавить любой из этих атрибутов в карточку профиля, настроив [параметры организации](/graph/api/resources/organizationsettings) и добавив атрибут в качестве свойства **directoryPropertyName** ресурса **profileCardProperty** в Microsoft Graph. Когда вы делаете дополнительные атрибуты видимыми, вы должны использовать имена свойств в формате `en-us`. Вам не требуется добавлять локализованные значения. Дополнительные свойства будут автоматически отображаться с использованием языковых настроек, указанных пользователем в Microsoft 365.

> [!IMPORTANT]
> При добавлении атрибута в карточку профиля его отображение занимает до 24 часов.

### <a name="example"></a>Пример

В следующем примере в карточке профиля отображается атрибут `Alias`.

``` http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

При успешном выполнении возвращается код отклика `201 OK` и объект **profileCardProperty** в тексте отклика. Значение атрибута `Alias` отображается в карточке профиля пользователя.

``` http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-a-custom-attribute"></a>Добавление настраиваемого атрибута

Вы можете добавлять в карточки профилей пользователей любой из 15 [настраиваемых атрибутов расширений](/graph/api/resources/onpremisesextensionattributes) Azure AD путем настройки параметров организации и [добавления соответствующего значения в качестве profileCardProperty](/graph/api/organizationsettings-post-profilecardproperties) в Microsoft Graph. Одновременно можно добавлять только один ресурс **profileCardProperty**.

Отображение внесенных изменений в карточках профилей занимают до 24 часов.

Настраиваемые свойства не поддерживают поиск, и их невозможно использовать для поиска людей в различных приложениях и службах Майкрософт.

В таблице ниже показано, как имена настраиваемых атрибутов расширений Azure AD соответствуют поддерживаемым значениям свойства **directoryPropertyName** ресурса [profileCardProperty](/graph/api/resources/profilecardproperty). В этих именах *регистр не учитывается*:

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

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Отклик

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
## <a name="deleting-a-custom-attribute"></a>Удаление настраиваемого атрибута

Следуя аналогичному сопоставлению между настраиваемыми атрибутами расширения Azure AD и настраиваемыми атрибутами карточки профиля (например, `customAttribute1`), как описано в предыдущем разделе [Добавление настраиваемого атрибута](/graph/add-properties-profilecard#adding-a-custom-attribute), вы можете удалить настраиваемый атрибут с помощью операции [удаления](/graph/api/profilecardproperty-delete?view=graph-rest-beta&preserve-view=true), как показано в примере ниже:

### <a name="example"></a>Пример

В следующем примере настраиваемый атрибут `customAttribute5` удаляется из параметров организации. После успешного удаления возвращается `HTTP 204`.

#### <a name="request"></a>Запрос

``` http
DELETE https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/customAttribute5
```

#### <a name="response"></a>Отклик

``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>См. также

- [Поиск идентификатора клиента Microsoft 365](/onedrive/find-your-office-365-tenant-id)
- [Тип ресурса onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes)
- [Тип ресурса user](/graph/api/resources/user)
- [Песочница Graph](https://developer.microsoft.com/graph/graph-explorer)
- [Получение ресурса profileCardProperty](/graph/api/profilecardproperty-get)
