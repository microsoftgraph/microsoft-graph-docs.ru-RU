---
title: 'Информатионпротектионлабел: Евалуатеаппликатион'
description: Определите, какую метку применить, на основе существующей информации о содержимом и желаемого состояния контента.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 76f57449f7e45a3616ccc45be1b329fe7ecbb928
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216689"
---
# <a name="informationprotectionlabel-evaluateapplication"></a><span data-ttu-id="e2f1d-103">Информатионпротектионлабел: Евалуатеаппликатион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-103">informationProtectionLabel: evaluateApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2f1d-104">Вычисление [Метки защиты информации](../resources/informationprotectionlabel.md) , которая должна быть применена, и возврат набора действий, которые необходимо выполнить, чтобы правильно обозначить информацию.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-104">Compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="e2f1d-105">Этот API полезен, если метку следует задать вручную или явным образом пользователем или службой, а не на основе содержимого файлов.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-105">This API is useful when a label should be set manually or explicitly by a user or service, rather than automatically based on file contents.</span></span> 

<span data-ttu-id="e2f1d-106">В данном [контентинфо](../resources/contentInfo.md), который включает существующие [пары ключей и значений](../resources/keyvaluepair.md)метаданных содержимого, и [лабелингоптионс](../resources/labelingoptions.md) в качестве входных данных, API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="e2f1d-106">Given [contentInfo](../resources/contentInfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [labelingOptions](../resources/labelingoptions.md) as an input, the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) object that contains one of more of the following:</span></span> 

* [<span data-ttu-id="e2f1d-107">аддконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-107">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="e2f1d-108">аддконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-108">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="e2f1d-109">аддватермаркактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-109">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="e2f1d-110">апплилабелактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-110">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="e2f1d-111">Запис</span><span class="sxs-lookup"><span data-stu-id="e2f1d-111">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="e2f1d-112">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-112">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="e2f1d-113">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-113">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="e2f1d-114">протектадхокактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-114">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="e2f1d-115">протектбитемплатеактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-115">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="e2f1d-116">протектиондонотфорвардактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-116">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="e2f1d-117">рекоммендлабелактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-117">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="e2f1d-118">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-118">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="e2f1d-119">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-119">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="e2f1d-120">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-120">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="e2f1d-121">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="e2f1d-121">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="e2f1d-122">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f1d-122">Permissions</span></span>

<span data-ttu-id="e2f1d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2f1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2f1d-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2f1d-125">Permission type</span></span>                        | <span data-ttu-id="e2f1d-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2f1d-126">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e2f1d-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2f1d-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2f1d-128">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="e2f1d-128">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="e2f1d-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2f1d-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2f1d-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-130">Not supported.</span></span>                              |
| <span data-ttu-id="e2f1d-131">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e2f1d-131">Application</span></span>                            | <span data-ttu-id="e2f1d-132">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="e2f1d-132">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="e2f1d-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2f1d-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/informationprotection/policy/labels/evaluateApplication
POST /users/{id}/informationProtection/policy/labels/evaluateApplication
```

## <a name="request-headers"></a><span data-ttu-id="e2f1d-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2f1d-134">Request headers</span></span>

| <span data-ttu-id="e2f1d-135">Имя</span><span class="sxs-lookup"><span data-stu-id="e2f1d-135">Name</span></span>          | <span data-ttu-id="e2f1d-136">Описание</span><span class="sxs-lookup"><span data-stu-id="e2f1d-136">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e2f1d-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2f1d-137">Authorization</span></span> | <span data-ttu-id="e2f1d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-p103">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="e2f1d-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e2f1d-140">Content-type</span></span>  | <span data-ttu-id="e2f1d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-p104">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="e2f1d-143">User — Agent</span><span class="sxs-lookup"><span data-stu-id="e2f1d-143">User-Agent</span></span>    | <span data-ttu-id="e2f1d-144">Описывает имя вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-144">Describes the name of the calling application.</span></span> <span data-ttu-id="e2f1d-145">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-145">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="e2f1d-146">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-146">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="e2f1d-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-147">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2f1d-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2f1d-148">Request body</span></span>

<span data-ttu-id="e2f1d-149">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-149">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e2f1d-150">Параметр</span><span class="sxs-lookup"><span data-stu-id="e2f1d-150">Parameter</span></span>       | <span data-ttu-id="e2f1d-151">Тип</span><span class="sxs-lookup"><span data-stu-id="e2f1d-151">Type</span></span>                                               | <span data-ttu-id="e2f1d-152">Описание</span><span class="sxs-lookup"><span data-stu-id="e2f1d-152">Description</span></span>                                                                                                                      |
| :-------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e2f1d-153">контентинфо</span><span class="sxs-lookup"><span data-stu-id="e2f1d-153">contentInfo</span></span>     | [<span data-ttu-id="e2f1d-154">контентинфо</span><span class="sxs-lookup"><span data-stu-id="e2f1d-154">contentInfo</span></span>](../resources/contentinfo.md)         | <span data-ttu-id="e2f1d-155">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e2f1d-155">Provides details on the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="e2f1d-156">лабелингоптионс</span><span class="sxs-lookup"><span data-stu-id="e2f1d-156">labelingOptions</span></span> | [<span data-ttu-id="e2f1d-157">лабелингоптионс</span><span class="sxs-lookup"><span data-stu-id="e2f1d-157">labelingOptions</span></span>](../resources/labelingoptions.md) | <span data-ttu-id="e2f1d-158">Предоставляет сведения о желаемом состоянии контента.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-158">Provides details about the desired state of the content.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="e2f1d-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2f1d-159">Response</span></span>

<span data-ttu-id="e2f1d-160">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-160">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2f1d-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="e2f1d-161">Examples</span></span>

<span data-ttu-id="e2f1d-162">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-162">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e2f1d-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2f1d-163">Request</span></span>

<span data-ttu-id="e2f1d-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-164">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2f1d-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2f1d-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateapplication"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateApplication
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2f1d-166">C#</span><span class="sxs-lookup"><span data-stu-id="e2f1d-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2f1d-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2f1d-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2f1d-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2f1d-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2f1d-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2f1d-169">Response</span></span>

<span data-ttu-id="e2f1d-170">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-170">The following is an example of the response.</span></span>

> <span data-ttu-id="e2f1d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2f1d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
