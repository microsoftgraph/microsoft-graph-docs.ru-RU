---
title: 'Информатионпротектионлабел: Евалуатеремовал'
description: Определите, какую метку удалить, и как ее удалить на основе существующей информации о контенте.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca1a27b30152debe51add8f0b418d3983c13b746
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995949"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="df7c3-103">Информатионпротектионлабел: Евалуатеремовал</span><span class="sxs-lookup"><span data-stu-id="df7c3-103">informationProtectionLabel: evaluateRemoval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df7c3-104">Укажите, какие действия необходимо предпринять для удаления сведений о наклейках в приложении, используемом для использования.</span><span class="sxs-lookup"><span data-stu-id="df7c3-104">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="df7c3-105">В [качестве](../resources/contentinfo.md) входных данных, которые включают существующие [пары ключ/значение](../resources/keyvaluepair.md)метаданных содержимого, API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит несколько комбинаций одного из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="df7c3-105">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="df7c3-106">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="df7c3-106">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="df7c3-107">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="df7c3-107">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="df7c3-108">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="df7c3-108">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="df7c3-109">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="df7c3-109">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="df7c3-110">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="df7c3-110">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="df7c3-111">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="df7c3-111">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="df7c3-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df7c3-112">Permissions</span></span>

<span data-ttu-id="df7c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df7c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df7c3-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df7c3-115">Permission type</span></span>                        | <span data-ttu-id="df7c3-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df7c3-116">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="df7c3-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df7c3-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="df7c3-118">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="df7c3-118">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="df7c3-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df7c3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df7c3-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df7c3-120">Not supported.</span></span>                              |
| <span data-ttu-id="df7c3-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df7c3-121">Application</span></span>                            | <span data-ttu-id="df7c3-122">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="df7c3-122">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="df7c3-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df7c3-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="df7c3-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df7c3-124">Request headers</span></span>

| <span data-ttu-id="df7c3-125">Имя</span><span class="sxs-lookup"><span data-stu-id="df7c3-125">Name</span></span>          | <span data-ttu-id="df7c3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="df7c3-126">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="df7c3-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df7c3-127">Authorization</span></span> | <span data-ttu-id="df7c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df7c3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="df7c3-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df7c3-130">Content-type</span></span>  | <span data-ttu-id="df7c3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df7c3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df7c3-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df7c3-133">Request body</span></span>

<span data-ttu-id="df7c3-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="df7c3-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="df7c3-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="df7c3-135">Parameter</span></span>              | <span data-ttu-id="df7c3-136">Тип</span><span class="sxs-lookup"><span data-stu-id="df7c3-136">Type</span></span>                                                             | <span data-ttu-id="df7c3-137">Описание</span><span class="sxs-lookup"><span data-stu-id="df7c3-137">Description</span></span>                                                                                                                                                                                                   |
| :--------------------- | :--------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="df7c3-138">контентинфо</span><span class="sxs-lookup"><span data-stu-id="df7c3-138">contentInfo</span></span>            | [<span data-ttu-id="df7c3-139">контентинфо</span><span class="sxs-lookup"><span data-stu-id="df7c3-139">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="df7c3-140">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="df7c3-140">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="df7c3-141">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="df7c3-141">downgradeJustification</span></span> | [<span data-ttu-id="df7c3-142">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="df7c3-142">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="df7c3-143">Обоснование, которое должно быть предоставлено логикой пользователя или приложения.</span><span class="sxs-lookup"><span data-stu-id="df7c3-143">Justification that must be provided by the user or application logic.</span></span>                                                                                                                                         |


## <a name="response"></a><span data-ttu-id="df7c3-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="df7c3-144">Response</span></span>

<span data-ttu-id="df7c3-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df7c3-145">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="df7c3-146">[Объект информатионпротектионактион](../resources/informationprotectionaction.md) будет содержать объект [метадатаактион](../resources/metadataaction.md) , который информирует приложение о том, какие метаданные необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="df7c3-146">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="df7c3-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="df7c3-147">Examples</span></span>

<span data-ttu-id="df7c3-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="df7c3-148">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="df7c3-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="df7c3-149">Request</span></span>

<span data-ttu-id="df7c3-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df7c3-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df7c3-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="df7c3-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateremoval"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateRemoval
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
  "downgradeJustification": {
        "justificationMessage": "The information has been declassified.",
        "isDowngradeJustified": true
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="df7c3-152">C#</span><span class="sxs-lookup"><span data-stu-id="df7c3-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateremoval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df7c3-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df7c3-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateremoval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df7c3-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df7c3-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateremoval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df7c3-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="df7c3-155">Response</span></span>

<span data-ttu-id="df7c3-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df7c3-156">The following is an example of the response.</span></span>

> <span data-ttu-id="df7c3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df7c3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
