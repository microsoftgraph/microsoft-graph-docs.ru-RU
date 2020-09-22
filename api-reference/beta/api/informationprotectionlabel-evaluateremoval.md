---
title: 'Информатионпротектионлабел: Евалуатеремовал'
description: Определите, какую метку удалить, и как ее удалить на основе существующей информации о контенте.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8ebb93f02216f0db9d04130e8ba3b5ba07f5ea7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001486"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="1520d-103">Информатионпротектионлабел: Евалуатеремовал</span><span class="sxs-lookup"><span data-stu-id="1520d-103">informationProtectionLabel: evaluateRemoval</span></span>

<span data-ttu-id="1520d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1520d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1520d-105">Укажите, какие действия необходимо предпринять для удаления сведений о наклейках в приложении, используемом для использования.</span><span class="sxs-lookup"><span data-stu-id="1520d-105">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="1520d-106">В [качестве](../resources/contentinfo.md) входных данных, которые включают существующие [пары ключ/значение](../resources/keyvaluepair.md)метаданных содержимого, API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит несколько комбинаций одного из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="1520d-106">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="1520d-107">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="1520d-107">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="1520d-108">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="1520d-108">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="1520d-109">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="1520d-109">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="1520d-110">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="1520d-110">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="1520d-111">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="1520d-111">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="1520d-112">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="1520d-112">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="1520d-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1520d-113">Permissions</span></span>

<span data-ttu-id="1520d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1520d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1520d-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1520d-116">Permission type</span></span>                        | <span data-ttu-id="1520d-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1520d-117">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1520d-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1520d-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="1520d-119">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="1520d-119">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="1520d-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1520d-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1520d-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1520d-121">Not supported.</span></span>                              |
| <span data-ttu-id="1520d-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1520d-122">Application</span></span>                            | <span data-ttu-id="1520d-123">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="1520d-123">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="1520d-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1520d-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="1520d-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1520d-125">Request headers</span></span>

| <span data-ttu-id="1520d-126">Имя</span><span class="sxs-lookup"><span data-stu-id="1520d-126">Name</span></span>          | <span data-ttu-id="1520d-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1520d-127">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1520d-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1520d-128">Authorization</span></span> | <span data-ttu-id="1520d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1520d-p102">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="1520d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1520d-131">Content-type</span></span>  | <span data-ttu-id="1520d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1520d-p103">application/json. Required.</span></span>                                                                                                                                                       |
| <span data-ttu-id="1520d-134">User — Agent</span><span class="sxs-lookup"><span data-stu-id="1520d-134">User-Agent</span></span>    | <span data-ttu-id="1520d-135">Описывает имя и версию вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="1520d-135">Describes the name and version of the calling application.</span></span> <span data-ttu-id="1520d-136">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="1520d-136">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="1520d-137">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="1520d-137">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="1520d-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1520d-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1520d-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1520d-139">Request body</span></span>

<span data-ttu-id="1520d-140">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1520d-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1520d-141">Параметр</span><span class="sxs-lookup"><span data-stu-id="1520d-141">Parameter</span></span>              | <span data-ttu-id="1520d-142">Тип</span><span class="sxs-lookup"><span data-stu-id="1520d-142">Type</span></span>                                                             | <span data-ttu-id="1520d-143">Описание</span><span class="sxs-lookup"><span data-stu-id="1520d-143">Description</span></span>                                                                                                                         |
| :--------------------- | :--------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1520d-144">контентинфо</span><span class="sxs-lookup"><span data-stu-id="1520d-144">contentInfo</span></span>            | [<span data-ttu-id="1520d-145">контентинфо</span><span class="sxs-lookup"><span data-stu-id="1520d-145">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="1520d-146">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="1520d-146">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="1520d-147">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="1520d-147">downgradeJustification</span></span> | [<span data-ttu-id="1520d-148">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="1520d-148">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="1520d-149">Обоснование, которое должно быть предоставлено логикой пользователя или приложения.</span><span class="sxs-lookup"><span data-stu-id="1520d-149">Justification that must be provided by the user or application logic.</span></span>                                                               |


## <a name="response"></a><span data-ttu-id="1520d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1520d-150">Response</span></span>

<span data-ttu-id="1520d-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1520d-151">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="1520d-152">[Объект информатионпротектионактион](../resources/informationprotectionaction.md) будет содержать объект [метадатаактион](../resources/metadataaction.md) , который информирует приложение о том, какие метаданные необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="1520d-152">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="1520d-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="1520d-153">Examples</span></span>

<span data-ttu-id="1520d-154">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1520d-154">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1520d-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="1520d-155">Request</span></span>

<span data-ttu-id="1520d-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1520d-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1520d-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="1520d-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1520d-158">C#</span><span class="sxs-lookup"><span data-stu-id="1520d-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateremoval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1520d-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1520d-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateremoval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1520d-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1520d-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateremoval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1520d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="1520d-161">Response</span></span>

<span data-ttu-id="1520d-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1520d-162">The following is an example of the response.</span></span>

> <span data-ttu-id="1520d-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1520d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


