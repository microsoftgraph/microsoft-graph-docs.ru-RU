---
title: 'informationProtectionLabel: evaluateClassificationResults'
description: Оцените, какую метку применять на основе существующих данных о контенте и результата классификации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 46fdfc7ad1cfd798ecaf8685e1473da09701c1c1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960949"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a><span data-ttu-id="23ddd-103">informationProtectionLabel: evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="23ddd-103">informationProtectionLabel: evaluateClassificationResults</span></span>

<span data-ttu-id="23ddd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23ddd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23ddd-105">С [помощью результатов](../resources/classificationresult.md) [](../resources/informationprotectionlabel.md) классификации вычислите метку защиты информации, которая должна быть применена, и верните набор действий, которые необходимо принять для правильной маркировки сведений.</span><span class="sxs-lookup"><span data-stu-id="23ddd-105">Using [classification results](../resources/classificationresult.md), compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="23ddd-106">Этот API полезен, когда метка должна быть заданной автоматически на основе классификации содержимого файла, а не метки непосредственно пользователем или службой.</span><span class="sxs-lookup"><span data-stu-id="23ddd-106">This API is useful when a label should be set automatically based on classification of the file contents, rather than labeled directly by a user or service.</span></span> 

<span data-ttu-id="23ddd-107">Чтобы оценить на основе результатов классификации, предостаточная [оценка контентаInfo,](../resources/contentinfo.md)который включает существующие пары [ключей/значений](../resources/keyvaluepair.md)метаданных контента и [результаты классификации.](../resources/classificationresult.md)</span><span class="sxs-lookup"><span data-stu-id="23ddd-107">To evaluate based on classification results, provide [contentInfo](../resources/contentinfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [classification results](../resources/classificationresult.md).</span></span> <span data-ttu-id="23ddd-108">API возвращает [informationProtectionAction,](../resources/informationprotectionaction.md) который содержит один из следующих ниже:</span><span class="sxs-lookup"><span data-stu-id="23ddd-108">The API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains one of more of the following:</span></span> 

* [<span data-ttu-id="23ddd-109">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-109">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="23ddd-110">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-110">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="23ddd-111">addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-111">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="23ddd-112">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-112">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="23ddd-113">customAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-113">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="23ddd-114">justifyAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-114">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="23ddd-115">metadataAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-115">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="23ddd-116">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-116">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="23ddd-117">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-117">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="23ddd-118">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-118">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="23ddd-119">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-119">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="23ddd-120">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-120">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="23ddd-121">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-121">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="23ddd-122">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-122">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="23ddd-123">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="23ddd-123">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="23ddd-124">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23ddd-124">Permissions</span></span>

<span data-ttu-id="23ddd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23ddd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23ddd-127">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23ddd-127">Permission type</span></span>                        | <span data-ttu-id="23ddd-128">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23ddd-128">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="23ddd-129">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23ddd-129">Delegated (work or school account)</span></span>     | <span data-ttu-id="23ddd-130">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="23ddd-130">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="23ddd-131">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23ddd-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23ddd-132">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ddd-132">Not supported.</span></span>                              |
| <span data-ttu-id="23ddd-133">Application</span><span class="sxs-lookup"><span data-stu-id="23ddd-133">Application</span></span>                            | <span data-ttu-id="23ddd-134">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="23ddd-134">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="23ddd-135">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23ddd-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a><span data-ttu-id="23ddd-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23ddd-136">Request headers</span></span>

| <span data-ttu-id="23ddd-137">Имя</span><span class="sxs-lookup"><span data-stu-id="23ddd-137">Name</span></span>          | <span data-ttu-id="23ddd-138">Описание</span><span class="sxs-lookup"><span data-stu-id="23ddd-138">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="23ddd-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23ddd-139">Authorization</span></span> | <span data-ttu-id="23ddd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23ddd-p104">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="23ddd-142">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23ddd-142">Content-type</span></span>  | <span data-ttu-id="23ddd-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23ddd-p105">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="23ddd-145">User-Agent</span><span class="sxs-lookup"><span data-stu-id="23ddd-145">User-Agent</span></span>    | <span data-ttu-id="23ddd-146">Описывает имя и версию вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="23ddd-146">Describes the name and version of the calling application.</span></span> <span data-ttu-id="23ddd-147">Сведения будут всплыть в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="23ddd-147">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="23ddd-148">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="23ddd-148">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="23ddd-149">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="23ddd-149">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23ddd-150">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23ddd-150">Request body</span></span>

<span data-ttu-id="23ddd-151">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="23ddd-151">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23ddd-152">Параметр</span><span class="sxs-lookup"><span data-stu-id="23ddd-152">Parameter</span></span>             | <span data-ttu-id="23ddd-153">Тип</span><span class="sxs-lookup"><span data-stu-id="23ddd-153">Type</span></span>                                                                    | <span data-ttu-id="23ddd-154">Описание</span><span class="sxs-lookup"><span data-stu-id="23ddd-154">Description</span></span>                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="23ddd-155">contentInfo</span><span class="sxs-lookup"><span data-stu-id="23ddd-155">contentInfo</span></span>           | [<span data-ttu-id="23ddd-156">contentInfo</span><span class="sxs-lookup"><span data-stu-id="23ddd-156">contentInfo</span></span>](../resources/contentInfo.md)                              | <span data-ttu-id="23ddd-157">Содержит сведения о формате контента, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в качестве пар ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="23ddd-157">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span>                                                                                                                                                   |
| <span data-ttu-id="23ddd-158">classificationResults</span><span class="sxs-lookup"><span data-stu-id="23ddd-158">classificationResults</span></span> | <span data-ttu-id="23ddd-159">[коллекция classificationResult](../resources/classificationresult.md)</span><span class="sxs-lookup"><span data-stu-id="23ddd-159">[classificationResult](../resources/classificationresult.md) collection</span></span> | <span data-ttu-id="23ddd-160">Содержит набор результатов классификации, возвращаемого конечной точкой классификации данных.</span><span class="sxs-lookup"><span data-stu-id="23ddd-160">Contains the set of classification results returned by the data classification endpoint.</span></span> <span data-ttu-id="23ddd-161">Сведения о классификации используются для определения соответствующей метки на основе конфигурации метки политики защиты информации Майкрософт в Центре безопасности и соответствия требованиям Office 365.</span><span class="sxs-lookup"><span data-stu-id="23ddd-161">Classification information is used to determine the appropriate label based on the Microsoft Information Protection policy label configuration in Office 365 Security and Compliance Center.</span></span> |

## <a name="response"></a><span data-ttu-id="23ddd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="23ddd-162">Response</span></span>

<span data-ttu-id="23ddd-163">В случае успешной работы этот метод возвращает код ответа и новый объект `200 OK` [коллекции informationProtectionAction](../resources/informationprotectionaction.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="23ddd-163">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23ddd-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="23ddd-164">Examples</span></span>

<span data-ttu-id="23ddd-165">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="23ddd-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="23ddd-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="23ddd-166">Request</span></span>

<span data-ttu-id="23ddd-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23ddd-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23ddd-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="23ddd-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="23ddd-169">C#</span><span class="sxs-lookup"><span data-stu-id="23ddd-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23ddd-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23ddd-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23ddd-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23ddd-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23ddd-172">Java</span><span class="sxs-lookup"><span data-stu-id="23ddd-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-evaluateclassificationresults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="23ddd-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="23ddd-173">Response</span></span>

<span data-ttu-id="23ddd-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23ddd-174">The following is an example of the response.</span></span>

> <span data-ttu-id="23ddd-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23ddd-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


