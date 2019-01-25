---
title: Обновление политики
description: Обновление свойств в уже существующей политики.
localization_priority: Normal
ms.openlocfilehash: d99aa42c4a67f6b874cbc1e266da76287388c05e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515414"
---
# <a name="update-policy"></a>Обновление политики

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств в уже существующей [политики](../resources/policy.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

```http
PATCH /policies/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type | application/json  | Характер данных в теле объекта. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите объект JSON вместе с параметрами, которые должны быть обновлены. В следующей таблице показаны возможные параметры.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|definition|String|Stringified версия объекта [политики](../resources/policy.md) .|
|displayName|String|Пользовательское имя для политики.|
|isOrganizationDefault|Логическое|Указывает, если эта политика будет применяться по умолчанию.|
|type|String|Указывает тип политики. В настоящее время должен быть «TokenLifetimePolicy»|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.

## <a name="example"></a>Пример
В следующем примере происходит обновление определения срока действия маркера и устанавливает ее в качестве организации по умолчанию.

##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
PATCH https://graph.microsoft.com/beta/policies/{id}
Content-Type: application/json
{
    "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
    "isOrganizationDefault":true
}
```

##### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.


```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
