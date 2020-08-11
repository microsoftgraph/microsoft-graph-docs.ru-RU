---
title: 'Информатионпротектионлабел: Евалуатеклассификатионресултс'
description: Определите, какую метку применить, на основе существующей информации о контенте и результата классификации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad1b8cc4c2792493e3ef511a9166c06c673482d6
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630272"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a>Информатионпротектионлабел: Евалуатеклассификатионресултс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используя [Результаты классификации](../resources/classificationresult.md), рассчитать [метку защиты информации](../resources/informationprotectionlabel.md) , которая должна быть применена, и возвратить набор действий, которые необходимо выполнить, чтобы правильно обозначить информацию. Этот API полезен, если метка должна быть задана автоматически на основе классификации содержимого файла, а не непосредственно пользователем или службой. 

Для оценки на основе результатов классификации предоставьте [контентинфо](../resources/contentinfo.md), включающий существующие [пары "ключ-значение" и "](../resources/keyvaluepair.md)метаданные контента", а также [Результаты классификации](../resources/classificationresult.md). API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит один из следующих элементов: 

* [аддконтентфутерактион](../resources/addcontentfooteraction.md)
* [аддконтенсеадерактион](../resources/addcontentheaderaction.md)
* [аддватермаркактион](../resources/addWatermarkaction.md)
* [апплилабелактион](../resources/applylabelaction.md)
* [Запис](../resources/customaction.md)
* [жустифяктион](../resources/justifyaction.md)
* [метадатаактион](../resources/metadataaction.md)
* [протектадхокактион](../resources/protectadhocaction.md)
* [протектбитемплатеактион](../resources/protectBytemplateaction.md)
* [протектиондонотфорвардактион](../resources/protectdonotforwardaction.md)
* [рекоммендлабелактион](../resources/recommendlabelaction.md)
* [ремовеконтентфутерактион](../resources/removecontentfooteraction.md)
* [ремовеконтенсеадерактион](../resources/removecontentheaderaction.md)
* [ремовепротектионактион](../resources/removeprotectionaction.md)
* [ремовеватермаркактион](../resources/removewatermarkaction.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированное (рабочая или учебная учетная запись)     | InformationProtectionPolicy.Read            |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | InformationProtectionPolicy.Read.All        |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Авторизация | Bearer {токен}. Обязательный.                                                                                                                                             |
| Content-Type  | application/json. Обязательный.                                                                                                                                           |
| User — Agent    | Описывает имя и версию вызывающего приложения. Подробные сведения отображаются в Azure Information Protection Analytics. Рекомендуемый формат — ApplicationName/Version. Необязательно. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр             | Тип                                                                    | Описание                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| контентинфо           | [контентинфо](../resources/contentInfo.md)                              | Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".                                                                                                                                                   |
| классификатионресултс | Коллекция [классификатионресулт](../resources/classificationresult.md) | Содержит набор результатов классификации, возвращаемых конечной точкой классификации данных. Сведения об классификации используются для определения соответствующей метки на основе конфигурации меток политики защиты информации Майкрософт в центре безопасности и соответствия требованиям Office 365. |

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.

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
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateClassificationResults
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

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

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
