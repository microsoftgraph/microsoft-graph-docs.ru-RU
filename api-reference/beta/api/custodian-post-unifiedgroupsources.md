---
title: Создание Унифиедграупсаурце
description: Создание нового объекта Унифиедграупсаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: f92fa2454b7ab20946091784af11b23ef2252acc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597738"
---
# <a name="create-unifiedgroupsource"></a>Создание Унифиедграупсаурце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [унифиедграупсаурце](../resources/unifiedgroupsource.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|User.Read|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/unifiedGroupSources
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [унифиедграупсаурце](../resources/unifiedgroupsource.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [унифиедграупсаурце](../resources/unifiedgroupsource.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|инклудедсаурцес|sourceType|Указывает, какие источники включены в эту группу. Возможные значения: `mailbox`, `site`.|
|group@odata. Bind|String|Идентификатор группы. Чтобы получить идентификатор группы, используйте операцию " [список групп](../api/group-list.md) ".|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [унифиедграупсаурце](../resources/unifiedgroupsource.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
Content-Type: application/json
Content-length: 219

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site"
}
```

### <a name="response"></a>Отклик

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedGroupSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "group@odata.bind": "/groups/000044f9-47c8-4a87-bccf-291fbf006a54",
  "includedSources":  "mailbox, site",
  "id": "14202dd90a1f4ccc84929586326c7104",
  "displayName": "SFA Videos",
  "createdDateTime": "2020-03-13T22:38:00.8985662Z",
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Megan Bowen"
      }
  }
}
```
