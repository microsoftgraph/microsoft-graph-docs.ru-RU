---
title: 'informationProtectionLabel: evaluateClassificationResults'
description: Оцените, какую метку применять на основе существующих данных о контенте и результата классификации.
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 26c65411ba7ce83fdae9d6d5ac46038deea84ac3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004794"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a>informationProtectionLabel: evaluateClassificationResults

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С [помощью результатов](../resources/classificationresult.md) [](../resources/informationprotectionlabel.md) классификации вычислите метку защиты информации, которая должна быть применена, и верните набор действий, которые необходимо принять для правильной маркировки сведений. Этот API полезен, когда метка должна быть заданной автоматически на основе классификации содержимого файла, а не метки непосредственно пользователем или службой. 

Чтобы оценить на основе результатов классификации, предостаточная [оценка контентаInfo,](../resources/contentinfo.md)который включает существующие пары [ключей/значений](../resources/keyvaluepair.md)метаданных контента и [результаты классификации.](../resources/classificationresult.md) API возвращает [informationProtectionAction,](../resources/informationprotectionaction.md) который содержит один из следующих ниже: 

* [addContentFooterAction](../resources/addcontentfooteraction.md)
* [addContentHeaderAction](../resources/addcontentheaderaction.md)
* [addWatermarkAction](../resources/addWatermarkaction.md)
* [applyLabelAction](../resources/applylabelaction.md)
* [customAction](../resources/customaction.md)
* [justifyAction](../resources/justifyaction.md)
* [metadataAction](../resources/metadataaction.md)
* [protectAdhocAction](../resources/protectadhocaction.md)
* [protectByTemplateAction](../resources/protectBytemplateaction.md)
* [protectionDoNotForwardAction](../resources/protectdonotforwardaction.md)
* [recommendLabelAction](../resources/recommendlabelaction.md)
* [removeContentFooterAction](../resources/removecontentfooteraction.md)
* [removeContentHeaderAction](../resources/removecontentheaderaction.md)
* [removeProtectionAction](../resources/removeprotectionaction.md)
* [removeWatermarkAction](../resources/removewatermarkaction.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | InformationProtectionPolicy.Read            |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | InformationProtectionPolicy.Read.All        |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Авторизация | Bearer {token}. Обязательный.                                                                                                                                             |
| Content-Type  | application/json. Обязательный.                                                                                                                                           |
| User-Agent    | Описывает имя и версию вызываемого приложения. Сведения будут всплыть в Azure Information Protection Analytics. Рекомендуемый формат — ApplicationName/Version. Необязательный параметр. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр             | Тип                                                                    | Описание                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| contentInfo           | [contentInfo](../resources/contentInfo.md)                              | Содержит сведения о формате контента, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в качестве пар ключей и значений.                                                                                                                                                   |
| classificationResults | [коллекция classificationResult](../resources/classificationresult.md) | Содержит набор результатов классификации, возвращаемого конечной точкой классификации данных. Сведения о классификации используются для определения соответствующей метки на основе конфигурации метки политик Microsoft Information Protection в центре Office 365 безопасности и соответствия требованиям. |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и новый объект `200 OK` [коллекции informationProtectionAction](../resources/informationprotectionaction.md) в тексте ответа.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateclassificationresults"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/evaluateClassificationResults
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
  "contentInfo": {
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "format": "default",
    "identifier": null,
    "state@odata.type": "#microsoft.graph.contentState",
    "state": "rest"
  },
  "classificationResults": [
    {
      "sensitiveTypeId": "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
      "count": 4,
      "confidenceLevel": 75
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-evaluateclassificationresults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/informationprotectionlabel-evaluateclassificationresults-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.informationProtectionAction)",
  "value": [
    {
      "@odata.type": "#microsoft.graph.applyLabelAction",
      "responsibleSensitiveTypeIds": [
        "cb353f78-2b72-4c3c-8827-92ebe4f69fdf"
      ],
      "actionSource": "automatic",
      "label": {
        "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
        "name": "Top Secret",
        "description": "",
        "color": "#000000",
        "sensitivity": 13,
        "tooltip": "This information is Top Secret.",
        "isActive": true
      },
      "actions": [
        {
          "@odata.type": "#microsoft.graph.protectByTemplateAction",
          "templateId": "0e7fea72-7bba-4438-a070-95c292cd6f8c"
        },
        {
          "@odata.type": "#microsoft.graph.metadataAction",
          "metadataToRemove": [],
          "metadataToAdd": [
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
              "value": "true"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
              "value": "2019-10-03T21:50:20Z"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
              "value": "Standard"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
              "value": "Top Secret"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
              "value": "cb46c030-1825-4e81-a295-151c039dbf02"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
              "value": "76dc494e-6c59-43e6-88a1-0000edd58fca"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
              "value": "8"
            }
          ]
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateClassificationResults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


