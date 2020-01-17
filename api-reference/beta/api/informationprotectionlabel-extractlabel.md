---
title: 'Информатионпротектионлабел: Екстрактлабел'
description: Получение Информатионпротектионконтентлабел с помощью метаданных из объекта с меткой.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c04849feac987eefef82eb3e069645406218ff1f
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216308"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="8da6e-103">Информатионпротектионлабел: Екстрактлабел</span><span class="sxs-lookup"><span data-stu-id="8da6e-103">informationProtectionLabel: extractLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8da6e-104">Используя метаданные, существующие на основе уже помеченных данных, разрешите метаданные в соответствии с определенными метками чувствительности.</span><span class="sxs-lookup"><span data-stu-id="8da6e-104">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="8da6e-105">Входные данные [контентинфо](../resources/contentinfo.md) разрешаются в [информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md).</span><span class="sxs-lookup"><span data-stu-id="8da6e-105">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="8da6e-106">Ресурс **[информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md)** представляет метку конфиденциальности, которая была применена к части данных.</span><span class="sxs-lookup"><span data-stu-id="8da6e-106">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="8da6e-107">объекты [информатионпротектионлабел](../resources/informationprotectionlabel.md) — это абстрактные метки, которые входят в политику организационных наклеек и могут быть применены к данным.</span><span class="sxs-lookup"><span data-stu-id="8da6e-107">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="8da6e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8da6e-108">Permissions</span></span>

<span data-ttu-id="8da6e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8da6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8da6e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8da6e-111">Permission type</span></span>                        | <span data-ttu-id="8da6e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8da6e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8da6e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8da6e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="8da6e-114">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="8da6e-114">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="8da6e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8da6e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8da6e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8da6e-116">Not supported.</span></span>                              |
| <span data-ttu-id="8da6e-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8da6e-117">Application</span></span>                            | <span data-ttu-id="8da6e-118">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8da6e-118">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="8da6e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8da6e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="8da6e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8da6e-120">Request headers</span></span>

| <span data-ttu-id="8da6e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8da6e-121">Name</span></span>          | <span data-ttu-id="8da6e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8da6e-122">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8da6e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8da6e-123">Authorization</span></span> | <span data-ttu-id="8da6e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8da6e-p104">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="8da6e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8da6e-126">Content-type</span></span>  | <span data-ttu-id="8da6e-127">Content-Type: Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="8da6e-127">Content-type: application/json.</span></span> <span data-ttu-id="8da6e-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="8da6e-128">Required.</span></span>                                                                                                                                         |
| <span data-ttu-id="8da6e-129">User — Agent</span><span class="sxs-lookup"><span data-stu-id="8da6e-129">User-Agent</span></span>    | <span data-ttu-id="8da6e-130">Описывает имя и версию вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="8da6e-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="8da6e-131">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="8da6e-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="8da6e-132">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="8da6e-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="8da6e-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="8da6e-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8da6e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8da6e-134">Request body</span></span>

<span data-ttu-id="8da6e-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8da6e-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8da6e-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="8da6e-136">Parameter</span></span>   | <span data-ttu-id="8da6e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="8da6e-137">Type</span></span>                                       | <span data-ttu-id="8da6e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8da6e-138">Description</span></span>                                                                                                                         |
| :---------- | :----------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8da6e-139">контентинфо</span><span class="sxs-lookup"><span data-stu-id="8da6e-139">contentInfo</span></span> | [<span data-ttu-id="8da6e-140">контентинфо</span><span class="sxs-lookup"><span data-stu-id="8da6e-140">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="8da6e-141">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="8da6e-141">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="8da6e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da6e-142">Response</span></span>

<span data-ttu-id="8da6e-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8da6e-143">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8da6e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="8da6e-144">Examples</span></span>

<span data-ttu-id="8da6e-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8da6e-145">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8da6e-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8da6e-146">Request</span></span>

<span data-ttu-id="8da6e-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8da6e-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8da6e-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8da6e-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/extractLabel
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
                "value": "Top Secret"
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
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8da6e-149">C#</span><span class="sxs-lookup"><span data-stu-id="8da6e-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8da6e-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8da6e-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8da6e-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8da6e-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8da6e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8da6e-152">Response</span></span>

<span data-ttu-id="8da6e-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8da6e-153">The following is an example of the response.</span></span>

> <span data-ttu-id="8da6e-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8da6e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionContentLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.informationProtectionContentLabel",
    "creationDateTime": "1970-01-01T00:00:00Z",
    "assignmentMethod": "standard",
    "label": {
        "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
        "name": "Top Secret",
        "description": "",
        "color": "#000000",
        "sensitivity": 13,
        "tooltip": "This information is top secret.",
        "isActive": true
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: extractLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
