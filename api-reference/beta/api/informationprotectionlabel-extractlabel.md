---
title: 'Информатионпротектионлабел: Екстрактлабел'
description: Получение Информатионпротектионконтентлабел с помощью метаданных из объекта с меткой.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fe074f5dfa27dbad6b5415f3c75d5458665d2ea
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938024"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="cb7e6-103">Информатионпротектионлабел: Екстрактлабел</span><span class="sxs-lookup"><span data-stu-id="cb7e6-103">informationProtectionLabel: extractLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb7e6-104">Используя метаданные, существующие на основе уже помеченных данных, разрешите метаданные в соответствии с определенными метками чувствительности.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-104">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="cb7e6-105">Входные данные [контентинфо](../resources/contentinfo.md) разрешаются в [информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md).</span><span class="sxs-lookup"><span data-stu-id="cb7e6-105">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="cb7e6-106">Ресурс **[информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md)** представляет метку конфиденциальности, которая была применена к части данных.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-106">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="cb7e6-107">объекты [информатионпротектионлабел](../resources/informationprotectionlabel.md) — это абстрактные метки, которые входят в политику организационных наклеек и могут быть применены к данным.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-107">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb7e6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb7e6-108">Permissions</span></span>

<span data-ttu-id="cb7e6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb7e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb7e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb7e6-111">Permission type</span></span>                        | <span data-ttu-id="cb7e6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb7e6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cb7e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb7e6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb7e6-114">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="cb7e6-114">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="cb7e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb7e6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb7e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-116">Not supported.</span></span>                              |
| <span data-ttu-id="cb7e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb7e6-117">Application</span></span>                            | <span data-ttu-id="cb7e6-118">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="cb7e6-118">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="cb7e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb7e6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="cb7e6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb7e6-120">Request headers</span></span>

| <span data-ttu-id="cb7e6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="cb7e6-121">Name</span></span>          | <span data-ttu-id="cb7e6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cb7e6-122">Description</span></span>                    |
| :------------ | :----------------------------- |
| <span data-ttu-id="cb7e6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb7e6-123">Authorization</span></span> | <span data-ttu-id="cb7e6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-p104">Bearer {token}. Required.</span></span>                 |
| <span data-ttu-id="cb7e6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb7e6-126">Content-type</span></span>  | <span data-ttu-id="cb7e6-127">Content-Type: Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-127">Content-type: application/json.</span></span> <span data-ttu-id="cb7e6-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb7e6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb7e6-129">Request body</span></span>

<span data-ttu-id="cb7e6-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cb7e6-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="cb7e6-131">Parameter</span></span>   | <span data-ttu-id="cb7e6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="cb7e6-132">Type</span></span>                                       | <span data-ttu-id="cb7e6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="cb7e6-133">Description</span></span>                                                                                                                                                                                                   |
| :---------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="cb7e6-134">контентинфо</span><span class="sxs-lookup"><span data-stu-id="cb7e6-134">contentInfo</span></span> | [<span data-ttu-id="cb7e6-135">контентинфо</span><span class="sxs-lookup"><span data-stu-id="cb7e6-135">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="cb7e6-136">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="cb7e6-136">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="cb7e6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb7e6-137">Response</span></span>

<span data-ttu-id="cb7e6-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [информатионпротектионконтентлабел](../resources/informationprotectioncontentlabel.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-138">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb7e6-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb7e6-139">Examples</span></span>

<span data-ttu-id="cb7e6-140">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cb7e6-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb7e6-141">Request</span></span>

<span data-ttu-id="cb7e6-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-142">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/extractLabel
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

### <a name="response"></a><span data-ttu-id="cb7e6-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb7e6-143">Response</span></span>

<span data-ttu-id="cb7e6-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-144">The following is an example of the response.</span></span>

> <span data-ttu-id="cb7e6-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb7e6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
