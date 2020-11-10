---
title: 'Информатионпротектионлабел: Екстрактлабел'
description: Получение Информатионпротектионконтентлабел с помощью метаданных из объекта с меткой.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aaa9fe32f9ca07efa9dc4703fe9b78ee61443239
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964722"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="10d9a-103">Информатионпротектионлабел: Екстрактлабел</span><span class="sxs-lookup"><span data-stu-id="10d9a-103">informationProtectionLabel: extractLabel</span></span>

<span data-ttu-id="10d9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10d9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10d9a-105">Используя метаданные, существующие на основе уже помеченных данных, разрешите метаданные в соответствии с определенными метками чувствительности.</span><span class="sxs-lookup"><span data-stu-id="10d9a-105">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="10d9a-106">Входные данные [контентинфо](../resources/contentinfo.md) разрешаются в [информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md).</span><span class="sxs-lookup"><span data-stu-id="10d9a-106">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="10d9a-107">Ресурс **[информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md)** представляет метку конфиденциальности, которая была применена к части данных.</span><span class="sxs-lookup"><span data-stu-id="10d9a-107">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="10d9a-108">объекты [информатионпротектионлабел](../resources/informationprotectionlabel.md) — это абстрактные метки, которые входят в политику организационных наклеек и могут быть применены к данным.</span><span class="sxs-lookup"><span data-stu-id="10d9a-108">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="10d9a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10d9a-109">Permissions</span></span>

<span data-ttu-id="10d9a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10d9a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10d9a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10d9a-112">Permission type</span></span>                        | <span data-ttu-id="10d9a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10d9a-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="10d9a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10d9a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="10d9a-115">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="10d9a-115">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="10d9a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10d9a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10d9a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10d9a-117">Not supported.</span></span>                              |
| <span data-ttu-id="10d9a-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="10d9a-118">Application</span></span>                            | <span data-ttu-id="10d9a-119">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="10d9a-119">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="10d9a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10d9a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="10d9a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10d9a-121">Request headers</span></span>

| <span data-ttu-id="10d9a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="10d9a-122">Name</span></span>          | <span data-ttu-id="10d9a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="10d9a-123">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="10d9a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10d9a-124">Authorization</span></span> | <span data-ttu-id="10d9a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10d9a-p104">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="10d9a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10d9a-127">Content-type</span></span>  | <span data-ttu-id="10d9a-128">Content-Type: Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="10d9a-128">Content-type: application/json.</span></span> <span data-ttu-id="10d9a-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10d9a-129">Required.</span></span>                                                                                                                                         |
| <span data-ttu-id="10d9a-130">User-Agent</span><span class="sxs-lookup"><span data-stu-id="10d9a-130">User-Agent</span></span>    | <span data-ttu-id="10d9a-131">Описывает имя и версию вызывающего приложения.</span><span class="sxs-lookup"><span data-stu-id="10d9a-131">Describes the name and version of the calling application.</span></span> <span data-ttu-id="10d9a-132">Подробные сведения отображаются в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="10d9a-132">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="10d9a-133">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="10d9a-133">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="10d9a-134">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="10d9a-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10d9a-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10d9a-135">Request body</span></span>

<span data-ttu-id="10d9a-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="10d9a-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="10d9a-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="10d9a-137">Parameter</span></span>   | <span data-ttu-id="10d9a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="10d9a-138">Type</span></span>                                       | <span data-ttu-id="10d9a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="10d9a-139">Description</span></span>                                                                                                                         |
| :---------- | :----------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="10d9a-140">контентинфо</span><span class="sxs-lookup"><span data-stu-id="10d9a-140">contentInfo</span></span> | [<span data-ttu-id="10d9a-141">контентинфо</span><span class="sxs-lookup"><span data-stu-id="10d9a-141">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="10d9a-142">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="10d9a-142">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="10d9a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d9a-143">Response</span></span>

<span data-ttu-id="10d9a-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10d9a-144">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10d9a-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="10d9a-145">Examples</span></span>

<span data-ttu-id="10d9a-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="10d9a-146">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="10d9a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="10d9a-147">Request</span></span>

<span data-ttu-id="10d9a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10d9a-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="10d9a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="10d9a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/extractLabel
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
# <a name="c"></a>[<span data-ttu-id="10d9a-150">C#</span><span class="sxs-lookup"><span data-stu-id="10d9a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10d9a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10d9a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10d9a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10d9a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10d9a-153">Java</span><span class="sxs-lookup"><span data-stu-id="10d9a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-extractlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10d9a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="10d9a-154">Response</span></span>

<span data-ttu-id="10d9a-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10d9a-155">The following is an example of the response.</span></span>

> <span data-ttu-id="10d9a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10d9a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


