---
title: Удаление learningContent
description: Удаление объекта learningContent.
author: malabikaroy
ms.localizationpriority: medium
ms.prod: employee-learning
doc_type: apiPageType
ms.openlocfilehash: d3cc6df2fff5b4c7f80207d4b3f48ab13c08ae2e
ms.sourcegitcommit: d6d36ffd02bfd925343b11ab11dd735b3193740b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66883399"
---
# <a name="delete-learningcontent"></a>Удаление learningContent
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удалите указанный [ресурс learningContent](../resources/learningcontent.md) , представляющий метаданные принимаемых содержимого указанного поставщика.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|LearningContent.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|LearningContent.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /employeeExperience/learningProviders/{learningProviderId}/learningContents/{externalId='{externalId}'}/$ref
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "delete_learningcontent"
}
-->
``` http
DELETE /employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70/learningContents(externalId='27rg2ifb28gf28')/$ref
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

