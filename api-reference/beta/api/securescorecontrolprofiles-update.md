---
title: Обновление объектов secureScoreControlProfiles
description: Обновление редактируемого свойства secureScoreControlProfiles в рамках любого интегрированного решения для изменения различных свойств, например, присвоенныхTo или tenantNote.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 6fee598a91d7153b98ca6e36bb9a21ff949e8b22
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787242"
---
# <a name="update-securescorecontrolprofiles"></a>Обновление объектов secureScoreControlProfiles

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление редактируемого **свойства secureScoreControlProfiles** в рамках любого интегрированного решения для изменения различных свойств, например, присвоенныхTo или **tenantNote.** 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Приложение | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {код}. Обязательно.|
|Prefer | return=representation. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON значений для соответствующих полей, которые должны быть обновлены. В следующей таблице перечислены поля, которые можно обновить для secureScoreControlProfile. Значения для существующих свойств, не включенных в тело запроса, не изменятся. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|assignedTo|String|Имя аналитика, на который назначен контроль для выполнения, выполнения или устранения.|
|tenantNote|String|Аналитик комментирует управление (для управления клиентом).|
|controlStateUpdates| String|Параметр управления, управляемый аналитиком. Возможные значения: `ignore`, `thirdParty`, `reviewed`.|


## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`.

Если используется необязательный заголовок запроса, метод возвращает код ответа и обновленный объект `200 OK` [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "controlStateUpdates": "controlStateUpdates-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securescorecontrolprofiles-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securescorecontrolprofiles-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securescorecontrolprofiles-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securescorecontrolprofiles-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже представлен пример успешного отклика.
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```




<!--
{
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


