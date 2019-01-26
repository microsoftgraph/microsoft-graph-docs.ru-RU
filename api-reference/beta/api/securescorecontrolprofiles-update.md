---
title: Обновление secureScoreControlProfiles
description: Обновите свойство редактируемого secureScoreControlProfiles в любой интегрированное решение для изменения различных свойств, например assignedTo или tenantNote.
localization_priority: Normal
ms.openlocfilehash: 2be11c6b369d9dc411afa5af2219c3bfa8605c8a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573363"
---
# <a name="update-securescorecontrolprofiles"></a>Обновление secureScoreControlProfiles

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите свойство редактируемого **secureScoreControlProfiles** в любой интегрированное решение для изменения различных свойств, например **assignedTo** или **tenantNote**.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |   SecurityEvents.ReadWrite.All.  |
|Делегированные (личная учетная запись Майкрософт) |  Не поддерживается.  |
|Для приложений | SecurityEvents.ReadWrite.All. |

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

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|assignedTo|Строка|Имя элемента управления аналитик назначается для рассмотрения, реализации или исправления.|
|tenantNote|Строка|Комментарии аналитик на элементе управления (для управления клиента).|
|controlStateUpdates| Строка|Аналитик, управляемых с помощью параметра на элементе управления. Возможные значения: `ignore`, `thirdParty`, `reviewed`.|


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

### <a name="response"></a>Отклик

Ниже представлен пример успешного отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfile",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securescorecontrolprofiles-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
