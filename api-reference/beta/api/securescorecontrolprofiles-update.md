---
title: Обновление secureScoreControlProfiles
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: afbfcd1889c55dd53241ff8d796bb3ab492b2acf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074804"
---
# <a name="update-securescorecontrolprofiles"></a>Обновление secureScoreControlProfiles

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обновите свойство редактируемого **secureScoreControlProfiles** в любой интегрированное решение для изменения различных свойств, например **assignedTo** или **tenantNote**.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All.  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложения | SecurityEvents.ReadWrite.All. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Authorization  | В заголовке указывается "Bearer {код}". Обязательный.|
|Prefer | Возвращает = представление. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите представление JSON значений для соответствующие поля, которые должны обновляться. В следующей таблице приведены поля, которые могут быть обновлены для secureScoreControlProfile. Значения для существующих свойств, которые не включены в тексте запроса остаются без изменений. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство   | Тип |Description|
|:---------------|:--------|:----------|
|assignedTo|String|Имя элемента управления аналитик назначается для рассмотрения, реализации или исправления.|
|tenantNote|String|Комментарии аналитик на элементе управления (для управления клиента).|
|controlStateUpdates| String|Аналитик, управляемых с помощью параметра на элементе управления. Возможные значения: `ignore`, `thirdParty`, `reviewed`.|


## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

Если используется запрос на необязательный заголовок, метод возвращает `200 OK` код ответа и обновленные [secureScoreControlProfiles](../resources/securescorecontrolprofiles.md) объект в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a>Ответ

Ниже приведен пример успешного ответа.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
