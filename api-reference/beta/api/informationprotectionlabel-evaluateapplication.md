---
title: 'informationProtectionLabel: evaluateApplication'
description: Оцените, какую метку применять на основе существующей информации о контенте и желаемого состояния контента.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: b48fd3e0137e90232b484acd142224a9a8cdc70c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960961"
---
# <a name="informationprotectionlabel-evaluateapplication"></a><span data-ttu-id="a40c8-103">informationProtectionLabel: evaluateApplication</span><span class="sxs-lookup"><span data-stu-id="a40c8-103">informationProtectionLabel: evaluateApplication</span></span>

<span data-ttu-id="a40c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a40c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a40c8-105">Вычислить [метку защиты](../resources/informationprotectionlabel.md) информации, которая должна применяться, и вернуть набор действий, которые необходимо принять для правильной метки информации.</span><span class="sxs-lookup"><span data-stu-id="a40c8-105">Compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="a40c8-106">Этот API полезен, когда метка должна быть заданной пользователем или службой вручную или явно, а не автоматически на основе содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="a40c8-106">This API is useful when a label should be set manually or explicitly by a user or service, rather than automatically based on file contents.</span></span> 

<span data-ttu-id="a40c8-107">Учитывая [contentInfo,](../resources/contentInfo.md)который включает существующие пары [ключей/значений](../resources/keyvaluepair.md)метаданных контента и [меткиOptions](../resources/labelingoptions.md) в качестве ввода, API возвращает объект [informationProtectionAction,](../resources/informationprotectionaction.md) содержащий один из следующих ниже:</span><span class="sxs-lookup"><span data-stu-id="a40c8-107">Given [contentInfo](../resources/contentInfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [labelingOptions](../resources/labelingoptions.md) as an input, the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) object that contains one of more of the following:</span></span> 

* [<span data-ttu-id="a40c8-108">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-108">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="a40c8-109">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-109">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="a40c8-110">addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-110">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="a40c8-111">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-111">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="a40c8-112">customAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-112">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="a40c8-113">justifyAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-113">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="a40c8-114">metadataAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-114">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="a40c8-115">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-115">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="a40c8-116">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-116">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="a40c8-117">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-117">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="a40c8-118">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-118">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="a40c8-119">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-119">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="a40c8-120">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-120">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="a40c8-121">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-121">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="a40c8-122">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="a40c8-122">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="a40c8-123">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a40c8-123">Permissions</span></span>

<span data-ttu-id="a40c8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a40c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a40c8-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a40c8-126">Permission type</span></span>                        | <span data-ttu-id="a40c8-127">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a40c8-127">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a40c8-128">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a40c8-128">Delegated (work or school account)</span></span>     | <span data-ttu-id="a40c8-129">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="a40c8-129">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="a40c8-130">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a40c8-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a40c8-131">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a40c8-131">Not supported.</span></span>                              |
| <span data-ttu-id="a40c8-132">Application</span><span class="sxs-lookup"><span data-stu-id="a40c8-132">Application</span></span>                            | <span data-ttu-id="a40c8-133">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="a40c8-133">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="a40c8-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a40c8-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/informationProtection/policy/labels/evaluateApplication
POST /users/{id}/informationProtection/policy/labels/evaluateApplication
```

## <a name="request-headers"></a><span data-ttu-id="a40c8-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a40c8-135">Request headers</span></span>

| <span data-ttu-id="a40c8-136">Имя</span><span class="sxs-lookup"><span data-stu-id="a40c8-136">Name</span></span>          | <span data-ttu-id="a40c8-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a40c8-137">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a40c8-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a40c8-138">Authorization</span></span> | <span data-ttu-id="a40c8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a40c8-p103">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="a40c8-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a40c8-141">Content-type</span></span>  | <span data-ttu-id="a40c8-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a40c8-p104">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="a40c8-144">User-Agent</span><span class="sxs-lookup"><span data-stu-id="a40c8-144">User-Agent</span></span>    | <span data-ttu-id="a40c8-145">Описывает имя вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="a40c8-145">Describes the name of the calling application.</span></span> <span data-ttu-id="a40c8-146">Сведения будут всплыть в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="a40c8-146">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="a40c8-147">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="a40c8-147">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="a40c8-148">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="a40c8-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a40c8-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a40c8-149">Request body</span></span>

<span data-ttu-id="a40c8-150">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a40c8-150">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a40c8-151">Параметр</span><span class="sxs-lookup"><span data-stu-id="a40c8-151">Parameter</span></span>       | <span data-ttu-id="a40c8-152">Тип</span><span class="sxs-lookup"><span data-stu-id="a40c8-152">Type</span></span>                                               | <span data-ttu-id="a40c8-153">Описание</span><span class="sxs-lookup"><span data-stu-id="a40c8-153">Description</span></span>                                                                                                                      |
| :-------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a40c8-154">contentInfo</span><span class="sxs-lookup"><span data-stu-id="a40c8-154">contentInfo</span></span>     | [<span data-ttu-id="a40c8-155">contentInfo</span><span class="sxs-lookup"><span data-stu-id="a40c8-155">contentInfo</span></span>](../resources/contentinfo.md)         | <span data-ttu-id="a40c8-156">Предоставляет сведения о формате контента, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в качестве пар ключей и значений.</span><span class="sxs-lookup"><span data-stu-id="a40c8-156">Provides details on the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="a40c8-157">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="a40c8-157">labelingOptions</span></span> | [<span data-ttu-id="a40c8-158">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="a40c8-158">labelingOptions</span></span>](../resources/labelingoptions.md) | <span data-ttu-id="a40c8-159">Предоставляет сведения о желаемом состоянии контента.</span><span class="sxs-lookup"><span data-stu-id="a40c8-159">Provides details about the desired state of the content.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="a40c8-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a40c8-160">Response</span></span>

<span data-ttu-id="a40c8-161">В случае успешной работы этот метод возвращает код ответа и новый объект `200 OK` [коллекции informationProtectionAction](../resources/informationprotectionaction.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a40c8-161">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a40c8-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="a40c8-162">Examples</span></span>

<span data-ttu-id="a40c8-163">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a40c8-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="a40c8-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="a40c8-164">Request</span></span>

<span data-ttu-id="a40c8-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a40c8-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a40c8-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="a40c8-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateapplication"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/evaluateApplication
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
  "contentInfo": {
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "format": "default",
    "identifier": null,
    "state@odata.type": "#microsoft.graph.contentState",
    "state": "rest",
    "metadata@odata.type": "#Collection(microsoft.graph.keyValuePair)",
    "metadata": [
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
        "value": "True"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
        "value": "Standard"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
        "value": "1/1/0001 12:00:00 AM"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
        "value": "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
        "value": "General"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
        "value": "0"
      },
      {
        "@odata.type": "#microsoft.graph.keyValuePair",
        "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
        "value": "00000000-0000-0000-0000-000000000000"
      }
    ]
  },
  "labelingOptions": {
    "@odata.type": "#microsoft.graph.labelingOptions",
    "assignmentMethod@odata.type": "#microsoft.graph.assignmentMethod",
    "assignmentMethod": "standard",
    "labelId@odata.type": "#Guid",
    "labelId": "97309856-9c28-4ac6-9382-5f8bc20c457b",
    "downgradeJustification": null,
    "extendedProperties@odata.type": "#Collection(microsoft.graph.keyValuePair)",
    "extendedProperties": []
  }
}
```
# <a name="c"></a>[<span data-ttu-id="a40c8-167">C#</span><span class="sxs-lookup"><span data-stu-id="a40c8-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a40c8-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a40c8-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a40c8-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a40c8-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a40c8-170">Java</span><span class="sxs-lookup"><span data-stu-id="a40c8-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-evaluateapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a40c8-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="a40c8-171">Response</span></span>

<span data-ttu-id="a40c8-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a40c8-172">The following is an example of the response.</span></span>

> <span data-ttu-id="a40c8-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a40c8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "@odata.type": "#microsoft.graph.protectByTemplateAction",
            "templateId": "31f2f3ba-1a56-48b7-ad90-0edc774ccfa2"
        },
        {
            "@odata.type": "#microsoft.graph.metadataAction",
            "metadataToRemove": [
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"
            ],
            "metadataToAdd": [
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Enabled",
                    "value": "true"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_SetDate",
                    "value": "2019-10-03T21:40:02Z"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Method",
                    "value": "Standard"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Name",
                    "value": "Inspire Demo"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_SiteId",
                    "value": "cb46c030-1825-4e81-a295-151c039dbf02"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_ActionId",
                    "value": "987357d3-6512-46b5-b20e-000065400015"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_ContentBits",
                    "value": "8"
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
  "description": "informationProtectionLabel: evaluateApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


