---
title: Настройка карточки профиля с помощью API профилей в Microsoft Graph (Предварительная версия)
description: В этой статье описывается, как можно настроить карточку профиля, сделав дополнительные атрибуты видимыми, или добавить настраиваемые атрибуты.
author: PollyNincevic
localization_priority: Priority
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: dc0c78ecfdf00488c7c9c12969eea8b405be496c
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050979"
---
# <a name="add-additional-properties-to-the-profile-card-using-the-profile-api-in-microsoft-graph-preview"></a>Добавление дополнительных свойств в карточку профиля с помощью API профилей в Microsoft Graph (Предварительная версия)

В [карточке профиля](https://support.office.com/article/profile-cards-in-office-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501) в Microsoft 365 можно найти сведения о пользователях, которые хранятся и поддерживаются организацией, например **названием должности** или **местоположением офиса**.

Используйте ресурс [профилекардпроперти](/graph/api/resources/profilecardproperty?view=graph-rest-beta) для отображения дополнительных свойств из Azure AD в карточках профилей для Организации, выполнив следующие действия:

- Отображение дополнительных атрибутов

- Добавление настраиваемых атрибутов

Дополнительные свойства будут отображаться в разделе **контакт** карточки профиля в Microsoft 365.

> [!NOTE]
>Для выполнения операций над ресурсом **профилекардпроперти** , использующим делегированные разрешения, необходимо, чтобы вошедшего в систему пользователя была назначена роль "Администратор клиента" или "Глобальный администратор".

## <a name="make-additional-attributes-visible"></a>Сделать дополнительные атрибуты видимыми

Вы можете сделать следующие атрибуты из Azure Active Directory (Azure AD) видимыми в карточках профилей пользователей. В этих атрибутах *не учитывается регистр*:

- `UserPrincipalName`
- `Fax`
- `StreetAddress`
- `PostalCode`
- `StateOrProvince`
- `Alias`

В следующей таблице показано, как атрибуты Azure AD соответствуют свойствам объекта [пользователя](/graph/api/resources/user?view=graph-rest-beta) Microsoft Graph.

|Атрибут Azure AD |Свойство сущности пользователя|
|:---------------|:----------|
|UserPrincipalName|userPrincipalName |
|Факс|faxNumber|
|StreetAddress|streetAddress|
|PostalCode|postalCode|
|StateOrProvince|состояние
|Alias|mailNickname

Вы можете добавить любой из этих атрибутов в карточку профиля, настроив [Параметры организации](/graph/api/resources/organizationsettings?view=graph-rest-beta) и добавив атрибут в качестве свойства *Директорипропертинаме** объекта **профилекардпроперти** в Microsoft Graph. Когда вы сделаете дополнительные атрибуты видимыми, необходимо использовать имена свойств для `en-us` . Вам не нужно добавлять локализованные значения. Дополнительные свойства будут автоматически отображаться в языковых параметрах, заданных пользователем для Microsoft 365.

> [!IMPORTANT]
> При добавлении атрибута в карточку профиля для отображения добавления потребуется до 24 часов.

## <a name="example"></a>Пример

В приведенном ниже примере показано, как отобразить `Alias` атрибут в карточке профиля:

```http
POST https://graph.microsoft.com/beta/organization/{tenantid}/settings/profileCardProperties
Content-Type: application/json

{
  "directoryPropertyName": "Alias"
}
```

В случае успеха ответ возвращает `201 OK` код отклика и объект **профилекардпроперти** в тексте отклика. Значение `Alias` атрибута будет отображаться на карточке профиля пользователя.  

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "directoryPropertyName": "Alias",
  "annotations": []
}
```

## <a name="adding-custom-attributes"></a>Добавление настраиваемых атрибутов

Вы можете добавить в карты профилей пользователей любое из 15 [настраиваемых атрибутов настраиваемого расширения](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta) Azure AD, настроив параметры организации и [добавив соответствующее значение в качестве Профилекардпроперти](/graph/api/organizationsettings-post-profilecardproperties?view=graph-rest-beta) в Microsoft Graph. Можно добавить один ресурс **профилекардпроперти** за раз.

Изменения, отображаемые в карточках профилей, занимают до 24 часов.

Настраиваемые свойства не поддерживают поиск и не могут использоваться для поиска людей в приложениях и службах Майкрософт.

В следующей таблице показано, как имена настраиваемых атрибутов расширения Azure AD соответствуют поддерживаемым значениям для свойства **директорипропертинаме** ресурса [профилекардпроперти](/graph/api/resources/profilecardproperty?view=graph-rest-beta) . В именах настраиваемых атрибутов настраиваемого расширения Azure AD *не учитывается регистр*:

|Настраиваемый атрибут расширения Azure AD | Значение для указания в качестве Директорипропертинаме |
|:--------------------|:-----------------|
| От extensionattribute1 | customAttribute1 |
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

## <a name="example"></a>Пример

В следующем примере первый атрибут настраиваемого расширения Azure AD добавляется в карточку профиля с использованием отображаемого имени **центра затрат**. Для пользователей, для которых в качестве языковых параметров задан немецкий, отображаемое имя будет **костенстелле**.

```http
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

Если язык не поддерживается, будет отображаться имя свойства со значением по умолчанию.  

В случае успеха ответ возвращает `201 OK` код отклика и объект **профилекардпроперти** в тексте отклика. В этом примере можно предположить, что в карточке профиля отображается **костенстелле** для всех пользователей, для которых в карточке профиля задан немецкий языковой параметр. Для всех остальных пользователей **центр затрат** будет отображаться в карточке профиля.

```http
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

[Поиск идентификатора клиента Microsoft 365](https://docs.microsoft.com/onedrive/find-your-office-365-tenant-id)

[Тип ресурса onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-beta)

[Тип ресурса "пользователь"](/graph/api/resources/user?view=graph-rest-beta)

[Проводник графиков](https://developer.microsoft.com/graph/graph-explorer)

[Получение Профилекардпроперти](/graph/api/profilecardproperty-get?view=graph-rest-beta)
