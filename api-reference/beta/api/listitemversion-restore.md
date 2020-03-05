---
author: JeremyKelley
description: Восстановление предыдущей версии ресурса ListItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.
ms.date: 09/10/2017
title: Восстановление предыдущей версии элемента списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 25e244c9dee5adb3b756f2c4bae38b292dc16679
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457094"
---
# <a name="restore-a-previous-version-of-a-listitem"></a>Восстановление предыдущей версии ресурса ListItem

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Восстановление предыдущей версии ресурса ListItem в качестве текущей версии. При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|            Тип разрешения             |         Разрешения (в порядке повышения привилегий)          |
| :------------------------------------- | :----------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |
| Делегированные (личная учетная запись Майкрософт) | Н/д                                                          |
| Для приложений                            | Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>Тело запроса

Тело запроса не требуется.

## <a name="example"></a>Пример

В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a>Отклик

При успешном выполнении вызова API возвращается отклик `204 No content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": []
}
-->
