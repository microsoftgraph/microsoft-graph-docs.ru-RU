---
title: Добавление пользовательских данных в ресурсы user с помощью открытых расширений
description: 'В этой статье рассматривается пример использования *открытых расширений*. '
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 4d66a008f253fd2097b4a9e8833022c825ee3db2
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944237"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a>Добавление пользовательских данных в ресурсы user с помощью открытых расширений
В этой статье рассматривается пример использования *открытых расширений*. 

Представьте, что вы разрабатываете приложение, доступное на множестве клиентских платформ, например на компьютерах и мобильных устройствах.  Вы хотите, чтобы пользователи могли настраивать интерфейс, чтобы он выглядел одинаково независимо от того, какое устройство они используют для входа в приложение. Это распространенное требование для приложений. 

Для этого сценария в этой статье показано, как:

1. добавить открытое расширение, представляющее данные перемещаемого профиля пользователя;
2. запросить данные у пользователя и вернуть перемещаемый профиль;
3. изменить данные перемещаемого профиля пользователя (значение открытого расширения);
4. удалить данные перемещаемого профиля пользователя.

>**Примечание.** В этой статье показано, как добавлять, считывать, обновлять и удалять открытые расширения для ресурса **user**. Эти методы также поддерживаются для типов ресурсов **administrativeUnit**, **contact**, **device**, **event**, **group**, **organizaton**, **post**, **todoTask** и **todoTaskList**.  
Вы можете обновлять примеры запросов, используя любые из этих типов ресурсов. Отклики, показанные в этих примерах, могут быть сокращены для удобства чтения. 

## <a name="1-add-roaming-profile-information"></a>1. Добавление данных перемещаемого профиля
Пользователь входит в приложение и настраивает его внешний вид.  Эти параметры приложения должны перемещаться, чтобы интерфейс выглядел одинаково на любом устройстве.  В этой статье мы рассмотрим, как добавить данные перемещаемого профиля в ресурс пользователя.

### <a name="request"></a>Запрос
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
### <a name="response"></a>Отклик
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a>2. Получение данных перемещаемого профиля
Когда пользователь входит в приложение с другого устройства, приложение может получить данные профиля пользователя, а также соответствующие параметры перемещения. Для этого можно получить ресурс пользователя и дополнить свойство навигации расширения.

### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
### <a name="response"></a>Отклик
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
>**Примечание.** Если у вас есть несколько расширений, вы можете отфильтровать их по свойству **id**, чтобы получить нужное расширение.

## <a name="3-change-roaming-profile-information"></a>3. Изменение данных перемещаемого профиля
Пользователь может изменить данные своего перемещаемого профиля. Это можно сделать с помощью запроса ```PATCH``` со значением открытого расширения. 

### <a name="request"></a>Запрос
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

### <a name="response"></a>Отклик
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a>4. Удаление перемещаемого профиля пользователя
Пользователь решает, что ему не больше не нужен перемещаемый профиль, и удаляет его. Это можно сделать с помощью запроса ```DELETE``` со значением открытого расширения.

### <a name="request"></a>Запрос
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

### <a name="response"></a>Отклик
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](extensibility-overview.md)
- [Добавление пользовательских данных в группы с помощью расширений схемы](extensibility-schema-groups.md)
- [Тип ресурса openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [Создание открытого расширения](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [Получение открытого расширения](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [Обновление открытого расширения](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [Удаление открытого расширения](/graph/api/opentypeextension-delete?view=graph-rest-1.0)
