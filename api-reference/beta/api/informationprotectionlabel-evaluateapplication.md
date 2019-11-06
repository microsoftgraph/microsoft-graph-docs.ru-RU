---
title: 'Информатионпротектионлабел: Евалуатеаппликатион'
description: Определите, какую метку применить, на основе существующей информации о содержимом и желаемого состояния контента.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92de4d75e93be416b255dfc43400b304938a9759
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994452"
---
# <a name="informationprotectionlabel-evaluateapplication"></a><span data-ttu-id="05bbc-103">Информатионпротектионлабел: Евалуатеаппликатион</span><span class="sxs-lookup"><span data-stu-id="05bbc-103">informationProtectionLabel: evaluateApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05bbc-104">Вычисление [Метки защиты информации](../resources/informationprotectionlabel.md) , которая должна быть применена, и возврат набора действий, которые необходимо выполнить, чтобы правильно обозначить информацию.</span><span class="sxs-lookup"><span data-stu-id="05bbc-104">Compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="05bbc-105">Этот API полезен, если метку следует задать вручную или явным образом пользователем или службой, а не на основе содержимого файлов.</span><span class="sxs-lookup"><span data-stu-id="05bbc-105">This API is useful when a label should be set manually or explicitly by a user or service, rather than automatically based on file contents.</span></span> 

<span data-ttu-id="05bbc-106">В данном [контентинфо](../resources/contentInfo.md), который включает существующие [пары ключей и значений](../resources/keyvaluepair.md)метаданных содержимого, и [лабелингоптионс](../resources/labelingoptions.md) в качестве входных данных, API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит один из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="05bbc-106">Given [contentInfo](../resources/contentInfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [labelingOptions](../resources/labelingoptions.md) as an input, the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) object that contains one of more of the following:</span></span> 

* [<span data-ttu-id="05bbc-107">аддконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-107">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="05bbc-108">аддконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-108">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="05bbc-109">аддватермаркактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-109">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="05bbc-110">апплилабелактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-110">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="05bbc-111">Запис</span><span class="sxs-lookup"><span data-stu-id="05bbc-111">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="05bbc-112">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="05bbc-112">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="05bbc-113">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-113">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="05bbc-114">протектадхокактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-114">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="05bbc-115">протектбитемплатеактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-115">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="05bbc-116">протектиондонотфорвардактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-116">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="05bbc-117">рекоммендлабелактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-117">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="05bbc-118">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-118">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="05bbc-119">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-119">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="05bbc-120">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-120">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="05bbc-121">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="05bbc-121">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="05bbc-122">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05bbc-122">Permissions</span></span>

<span data-ttu-id="05bbc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05bbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05bbc-125">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05bbc-125">Permission type</span></span>                        | <span data-ttu-id="05bbc-126">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05bbc-126">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="05bbc-127">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05bbc-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="05bbc-128">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="05bbc-128">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="05bbc-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05bbc-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05bbc-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05bbc-130">Not supported.</span></span>                              |
| <span data-ttu-id="05bbc-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05bbc-131">Application</span></span>                            | <span data-ttu-id="05bbc-132">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="05bbc-132">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="05bbc-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05bbc-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/informationprotection/policy/labels/evaluateApplication
POST /users/{id}/informationProtection/policy/labels/evaluateApplication
```

## <a name="request-headers"></a><span data-ttu-id="05bbc-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05bbc-134">Request headers</span></span>

| <span data-ttu-id="05bbc-135">Имя</span><span class="sxs-lookup"><span data-stu-id="05bbc-135">Name</span></span>          | <span data-ttu-id="05bbc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="05bbc-136">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="05bbc-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05bbc-137">Authorization</span></span> | <span data-ttu-id="05bbc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05bbc-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="05bbc-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05bbc-140">Content-type</span></span>  | <span data-ttu-id="05bbc-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05bbc-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05bbc-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05bbc-143">Request body</span></span>

<span data-ttu-id="05bbc-144">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="05bbc-144">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="05bbc-145">Параметр</span><span class="sxs-lookup"><span data-stu-id="05bbc-145">Parameter</span></span>       | <span data-ttu-id="05bbc-146">Тип</span><span class="sxs-lookup"><span data-stu-id="05bbc-146">Type</span></span>                                               | <span data-ttu-id="05bbc-147">Описание</span><span class="sxs-lookup"><span data-stu-id="05bbc-147">Description</span></span>                                                                                                                                                                                                   |
| :-------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="05bbc-148">контентинфо</span><span class="sxs-lookup"><span data-stu-id="05bbc-148">contentInfo</span></span>     | [<span data-ttu-id="05bbc-149">контентинфо</span><span class="sxs-lookup"><span data-stu-id="05bbc-149">contentInfo</span></span>](../resources/contentinfo.md)         | <span data-ttu-id="05bbc-150">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="05bbc-150">Provides details on the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="05bbc-151">лабелингоптионс</span><span class="sxs-lookup"><span data-stu-id="05bbc-151">labelingOptions</span></span> | [<span data-ttu-id="05bbc-152">лабелингоптионс</span><span class="sxs-lookup"><span data-stu-id="05bbc-152">labelingOptions</span></span>](../resources/labelingoptions.md) | <span data-ttu-id="05bbc-153">Предоставляет сведения о желаемом состоянии контента.</span><span class="sxs-lookup"><span data-stu-id="05bbc-153">Provides details about the desired state of the content.</span></span>                                                                                                                                                      |

## <a name="response"></a><span data-ttu-id="05bbc-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="05bbc-154">Response</span></span>

<span data-ttu-id="05bbc-155">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05bbc-155">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05bbc-156">Примеры</span><span class="sxs-lookup"><span data-stu-id="05bbc-156">Examples</span></span>

<span data-ttu-id="05bbc-157">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="05bbc-157">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="05bbc-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="05bbc-158">Request</span></span>

<span data-ttu-id="05bbc-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05bbc-159">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="05bbc-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="05bbc-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateapplication"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateApplication
Content-type: application/json

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
# <a name="ctabcsharp"></a>[<span data-ttu-id="05bbc-161">C#</span><span class="sxs-lookup"><span data-stu-id="05bbc-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05bbc-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05bbc-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05bbc-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05bbc-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05bbc-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="05bbc-164">Response</span></span>

<span data-ttu-id="05bbc-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05bbc-165">The following is an example of the response.</span></span>

> <span data-ttu-id="05bbc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05bbc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
