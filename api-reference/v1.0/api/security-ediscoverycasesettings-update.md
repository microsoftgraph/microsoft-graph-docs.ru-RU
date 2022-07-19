---
title: Обновление ediscoveryCaseSettings
description: Обновление свойств объекта ediscoveryCaseSettings.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 201264d2f03f6c2d92cdc49266b764f928d94773
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839968"
---
# <a name="update-ediscoverycasesettings"></a>Обновление ediscoveryCaseSettings
Пространство имен: microsoft.graph.security



Обновление свойств объекта [ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/settings
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса



|Свойство|Тип|Описание|
|:---|:---|:---|
|redundancyDetection|[microsoft.graph.security.redundancyDetectionSettings](../resources/security-redundancydetectionsettings.md)|Параметры избыточности (потоковая обработка электронной почты и обнаружение практически повторяющихся данных) для дела обнаружения электронных данных. Необязательный элемент.|
|topicModeling|[microsoft.graph.security.topicModelingSettings](../resources/security-topicmodelingsettings.md)|Параметры моделирования тем (тем) для дела обнаружения электронных данных. Необязательный элемент.|
|Ocr|[microsoft.graph.security.ocrSettings](../resources/security-ocrsettings.md)|Параметры OCR (оптическое распознавание символов) для дела обнаружения электронных данных. Необязательный параметр.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycasesettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/security/cases/ediscoveryCases/{ediscoveryCaseId}/settings
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.ediscoveryCaseSettings",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.security.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.security.ocrSettings"
  }
}
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