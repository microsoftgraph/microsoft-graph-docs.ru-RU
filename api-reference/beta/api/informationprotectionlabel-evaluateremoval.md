---
title: 'Информатионпротектионлабел: Евалуатеремовал'
description: Определите, какую метку удалить, и как ее удалить на основе существующей информации о контенте.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: acea1f8ba7021e76d069f8da60c7b5cb9bbe9604
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216717"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="f7520-103">Информатионпротектионлабел: Евалуатеремовал</span><span class="sxs-lookup"><span data-stu-id="f7520-103">informationProtectionLabel: evaluateRemoval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7520-104">Укажите, какие действия необходимо предпринять для удаления сведений о наклейках в приложении, используемом для использования.</span><span class="sxs-lookup"><span data-stu-id="f7520-104">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="f7520-105">В [качестве](../resources/contentinfo.md) входных данных, которые включают существующие [пары ключ/значение](../resources/keyvaluepair.md)метаданных содержимого, API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит несколько комбинаций одного из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="f7520-105">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="f7520-106">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="f7520-106">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="f7520-107">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="f7520-107">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="f7520-108">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="f7520-108">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="f7520-109">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="f7520-109">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="f7520-110">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="f7520-110">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="f7520-111">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="f7520-111">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="f7520-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7520-112">Permissions</span></span>

<span data-ttu-id="f7520-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7520-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7520-115">Permission type</span></span>                        | <span data-ttu-id="f7520-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7520-116">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f7520-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7520-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7520-118">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="f7520-118">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="f7520-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7520-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7520-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7520-120">Not supported.</span></span>                              |
| <span data-ttu-id="f7520-121">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f7520-121">Application</span></span>                            | <span data-ttu-id="f7520-122">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="f7520-122">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="f7520-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7520-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="f7520-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7520-124">Request headers</span></span>

| <span data-ttu-id="f7520-125">Имя</span><span class="sxs-lookup"><span data-stu-id="f7520-125">Name</span></span>          | <span data-ttu-id="f7520-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f7520-126">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f7520-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7520-127">Authorization</span></span> | <span data-ttu-id="f7520-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7520-p102">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="f7520-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7520-130">Content-type</span></span>  | <span data-ttu-id="f7520-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7520-p103">application/json. Required.</span></span>                                                                                                                                                       |
| <span data-ttu-id="f7520-133">User — Agent</span><span class="sxs-lookup"><span data-stu-id="f7520-133">User-Agent</span></span>    | <span data-ttu-id="f7520-134">Описывает имя и версию вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="f7520-134">Describes the name and version of the calling application.</span></span> <span data-ttu-id="f7520-135">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="f7520-135">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="f7520-136">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="f7520-136">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="f7520-137">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f7520-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7520-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7520-138">Request body</span></span>

<span data-ttu-id="f7520-139">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f7520-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7520-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="f7520-140">Parameter</span></span>              | <span data-ttu-id="f7520-141">Тип</span><span class="sxs-lookup"><span data-stu-id="f7520-141">Type</span></span>                                                             | <span data-ttu-id="f7520-142">Описание</span><span class="sxs-lookup"><span data-stu-id="f7520-142">Description</span></span>                                                                                                                         |
| :--------------------- | :--------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f7520-143">контентинфо</span><span class="sxs-lookup"><span data-stu-id="f7520-143">contentInfo</span></span>            | [<span data-ttu-id="f7520-144">контентинфо</span><span class="sxs-lookup"><span data-stu-id="f7520-144">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="f7520-145">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="f7520-145">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="f7520-146">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="f7520-146">downgradeJustification</span></span> | [<span data-ttu-id="f7520-147">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="f7520-147">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="f7520-148">Обоснование, которое должно быть предоставлено логикой пользователя или приложения.</span><span class="sxs-lookup"><span data-stu-id="f7520-148">Justification that must be provided by the user or application logic.</span></span>                                                               |


## <a name="response"></a><span data-ttu-id="f7520-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7520-149">Response</span></span>

<span data-ttu-id="f7520-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7520-150">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="f7520-151">[Объект информатионпротектионактион](../resources/informationprotectionaction.md) будет содержать объект [метадатаактион](../resources/metadataaction.md) , который информирует приложение о том, какие метаданные необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="f7520-151">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="f7520-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="f7520-152">Examples</span></span>

<span data-ttu-id="f7520-153">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f7520-153">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f7520-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7520-154">Request</span></span>

<span data-ttu-id="f7520-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7520-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7520-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7520-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateremoval"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateRemoval
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
  "downgradeJustification": {
        "justificationMessage": "The information has been declassified.",
        "isDowngradeJustified": true
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7520-157">C#</span><span class="sxs-lookup"><span data-stu-id="f7520-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateremoval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7520-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7520-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateremoval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7520-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7520-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateremoval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7520-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7520-160">Response</span></span>

<span data-ttu-id="f7520-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f7520-161">The following is an example of the response.</span></span>

> <span data-ttu-id="f7520-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f7520-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "metadataToAdd": []
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateRemoval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
