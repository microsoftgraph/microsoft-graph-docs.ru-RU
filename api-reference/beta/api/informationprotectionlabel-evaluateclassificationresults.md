---
title: 'Информатионпротектионлабел: Евалуатеклассификатионресултс'
description: Определите, какую метку применить, на основе существующей информации о контенте и результата классификации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46fc62d610a792493585dd3a5241e8af30d183ee
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932467"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a><span data-ttu-id="c1880-103">Информатионпротектионлабел: Евалуатеклассификатионресултс</span><span class="sxs-lookup"><span data-stu-id="c1880-103">informationProtectionLabel: evaluateClassificationResults</span></span>

<span data-ttu-id="c1880-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1880-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1880-105">Используя [Результаты классификации](../resources/classificationresult.md), рассчитать [метку защиты информации](../resources/informationprotectionlabel.md) , которая должна быть применена, и возвратить набор действий, которые необходимо выполнить, чтобы правильно обозначить информацию.</span><span class="sxs-lookup"><span data-stu-id="c1880-105">Using [classification results](../resources/classificationresult.md), compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="c1880-106">Этот API полезен, если метка должна быть задана автоматически на основе классификации содержимого файла, а не непосредственно пользователем или службой.</span><span class="sxs-lookup"><span data-stu-id="c1880-106">This API is useful when a label should be set automatically based on classification of the file contents, rather than labeled directly by a user or service.</span></span> 

<span data-ttu-id="c1880-107">Для оценки на основе результатов классификации предоставьте [контентинфо](../resources/contentinfo.md), включающий существующие [пары "ключ-значение" и "](../resources/keyvaluepair.md)метаданные контента", а также [Результаты классификации](../resources/classificationresult.md).</span><span class="sxs-lookup"><span data-stu-id="c1880-107">To evaluate based on classification results, provide [contentInfo](../resources/contentinfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [classification results](../resources/classificationresult.md).</span></span> <span data-ttu-id="c1880-108">API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="c1880-108">The API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains one of more of the following:</span></span> 

* [<span data-ttu-id="c1880-109">аддконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="c1880-109">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="c1880-110">аддконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="c1880-110">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="c1880-111">аддватермаркактион</span><span class="sxs-lookup"><span data-stu-id="c1880-111">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="c1880-112">апплилабелактион</span><span class="sxs-lookup"><span data-stu-id="c1880-112">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="c1880-113">Запис</span><span class="sxs-lookup"><span data-stu-id="c1880-113">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="c1880-114">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="c1880-114">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="c1880-115">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="c1880-115">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="c1880-116">протектадхокактион</span><span class="sxs-lookup"><span data-stu-id="c1880-116">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="c1880-117">протектбитемплатеактион</span><span class="sxs-lookup"><span data-stu-id="c1880-117">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="c1880-118">протектиондонотфорвардактион</span><span class="sxs-lookup"><span data-stu-id="c1880-118">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="c1880-119">рекоммендлабелактион</span><span class="sxs-lookup"><span data-stu-id="c1880-119">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="c1880-120">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="c1880-120">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="c1880-121">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="c1880-121">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="c1880-122">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="c1880-122">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="c1880-123">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="c1880-123">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="c1880-124">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1880-124">Permissions</span></span>

<span data-ttu-id="c1880-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1880-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1880-127">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1880-127">Permission type</span></span>                        | <span data-ttu-id="c1880-128">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1880-128">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c1880-129">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1880-129">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1880-130">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="c1880-130">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="c1880-131">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1880-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1880-132">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1880-132">Not supported.</span></span>                              |
| <span data-ttu-id="c1880-133">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1880-133">Application</span></span>                            | <span data-ttu-id="c1880-134">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1880-134">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="c1880-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1880-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a><span data-ttu-id="c1880-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1880-136">Request headers</span></span>

| <span data-ttu-id="c1880-137">Имя</span><span class="sxs-lookup"><span data-stu-id="c1880-137">Name</span></span>          | <span data-ttu-id="c1880-138">Описание</span><span class="sxs-lookup"><span data-stu-id="c1880-138">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c1880-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1880-139">Authorization</span></span> | <span data-ttu-id="c1880-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1880-p104">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="c1880-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1880-142">Content-type</span></span>  | <span data-ttu-id="c1880-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1880-p105">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="c1880-145">User-Agent</span><span class="sxs-lookup"><span data-stu-id="c1880-145">User-Agent</span></span>    | <span data-ttu-id="c1880-146">Описывает имя и версию вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="c1880-146">Describes the name and version of the calling application.</span></span> <span data-ttu-id="c1880-147">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="c1880-147">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="c1880-148">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="c1880-148">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="c1880-149">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c1880-149">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1880-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1880-150">Request body</span></span>

<span data-ttu-id="c1880-151">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c1880-151">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c1880-152">Параметр</span><span class="sxs-lookup"><span data-stu-id="c1880-152">Parameter</span></span>             | <span data-ttu-id="c1880-153">Тип</span><span class="sxs-lookup"><span data-stu-id="c1880-153">Type</span></span>                                                                    | <span data-ttu-id="c1880-154">Описание</span><span class="sxs-lookup"><span data-stu-id="c1880-154">Description</span></span>                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="c1880-155">контентинфо</span><span class="sxs-lookup"><span data-stu-id="c1880-155">contentInfo</span></span>           | [<span data-ttu-id="c1880-156">контентинфо</span><span class="sxs-lookup"><span data-stu-id="c1880-156">contentInfo</span></span>](../resources/contentInfo.md)                              | <span data-ttu-id="c1880-157">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="c1880-157">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span>                                                                                                                                                   |
| <span data-ttu-id="c1880-158">классификатионресултс</span><span class="sxs-lookup"><span data-stu-id="c1880-158">classificationResults</span></span> | <span data-ttu-id="c1880-159">Коллекция [классификатионресулт](../resources/classificationresult.md)</span><span class="sxs-lookup"><span data-stu-id="c1880-159">[classificationResult](../resources/classificationresult.md) collection</span></span> | <span data-ttu-id="c1880-160">Содержит набор результатов классификации, возвращаемых конечной точкой классификации данных.</span><span class="sxs-lookup"><span data-stu-id="c1880-160">Contains the set of classification results returned by the data classification endpoint.</span></span> <span data-ttu-id="c1880-161">Сведения об классификации используются для определения соответствующей метки на основе конфигурации меток политики защиты информации Майкрософт в центре безопасности и соответствия требованиям Office 365.</span><span class="sxs-lookup"><span data-stu-id="c1880-161">Classification information is used to determine the appropriate label based on the Microsoft Information Protection policy label configuration in Office 365 Security and Compliance Center.</span></span> |

## <a name="response"></a><span data-ttu-id="c1880-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1880-162">Response</span></span>

<span data-ttu-id="c1880-163">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1880-163">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1880-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1880-164">Examples</span></span>

<span data-ttu-id="c1880-165">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c1880-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c1880-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1880-166">Request</span></span>

<span data-ttu-id="c1880-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1880-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1880-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1880-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c1880-169">C#</span><span class="sxs-lookup"><span data-stu-id="c1880-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1880-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1880-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1880-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1880-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1880-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1880-172">Response</span></span>

<span data-ttu-id="c1880-173">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1880-173">The following is an example of the response.</span></span>

> <span data-ttu-id="c1880-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1880-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


