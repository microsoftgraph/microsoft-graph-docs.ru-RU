---
title: 'Информатионпротектионлабел: Евалуатеремовал'
description: Определите, какую метку удалить, и как ее удалить на основе существующей информации о контенте.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5d8723285ab364d7453d782806064e12de2b78f5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938543"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="8672e-103">Информатионпротектионлабел: Евалуатеремовал</span><span class="sxs-lookup"><span data-stu-id="8672e-103">informationProtectionLabel: evaluateRemoval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8672e-104">Укажите, какие действия необходимо предпринять для удаления сведений о наклейках в приложении, используемом для использования.</span><span class="sxs-lookup"><span data-stu-id="8672e-104">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="8672e-105">В [качестве](../resources/contentinfo.md) входных данных, которые включают существующие [пары ключ/значение](../resources/keyvaluepair.md)метаданных содержимого, API возвращает объект [информатионпротектионактион](../resources/informationprotectionaction.md) , который содержит несколько комбинаций одного из следующих элементов:</span><span class="sxs-lookup"><span data-stu-id="8672e-105">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="8672e-106">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="8672e-106">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="8672e-107">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="8672e-107">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="8672e-108">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="8672e-108">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="8672e-109">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="8672e-109">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="8672e-110">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="8672e-110">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="8672e-111">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="8672e-111">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="8672e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8672e-112">Permissions</span></span>

<span data-ttu-id="8672e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8672e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8672e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8672e-115">Permission type</span></span>                        | <span data-ttu-id="8672e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8672e-116">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8672e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8672e-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="8672e-118">Информатионпротектионполици. Read</span><span class="sxs-lookup"><span data-stu-id="8672e-118">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="8672e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8672e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8672e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8672e-120">Not supported.</span></span>                              |
| <span data-ttu-id="8672e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8672e-121">Application</span></span>                            | <span data-ttu-id="8672e-122">Информатионпротектионполици. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="8672e-122">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="8672e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8672e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="8672e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8672e-124">Request headers</span></span>

| <span data-ttu-id="8672e-125">Имя</span><span class="sxs-lookup"><span data-stu-id="8672e-125">Name</span></span>          | <span data-ttu-id="8672e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8672e-126">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="8672e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8672e-127">Authorization</span></span> | <span data-ttu-id="8672e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8672e-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="8672e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8672e-130">Content-type</span></span>  | <span data-ttu-id="8672e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8672e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8672e-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8672e-133">Request body</span></span>

<span data-ttu-id="8672e-134">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8672e-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8672e-135">Параметр</span><span class="sxs-lookup"><span data-stu-id="8672e-135">Parameter</span></span>              | <span data-ttu-id="8672e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="8672e-136">Type</span></span>                                                             | <span data-ttu-id="8672e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="8672e-137">Description</span></span>                                                                                                                                                                                                   |
| :--------------------- | :--------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="8672e-138">контентинфо</span><span class="sxs-lookup"><span data-stu-id="8672e-138">contentInfo</span></span>            | [<span data-ttu-id="8672e-139">контентинфо</span><span class="sxs-lookup"><span data-stu-id="8672e-139">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="8672e-140">Предоставляет подробные сведения о формате содержимого, состоянии контента и существующих [метаданных](../resources/keyvaluepair.md) в виде пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="8672e-140">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="8672e-141">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="8672e-141">downgradeJustification</span></span> | [<span data-ttu-id="8672e-142">довнградежустификатион</span><span class="sxs-lookup"><span data-stu-id="8672e-142">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="8672e-143">Обоснование, которое должно быть предоставлено логикой пользователя или приложения.</span><span class="sxs-lookup"><span data-stu-id="8672e-143">Justification that must be provided by the user or application logic.</span></span>                                                                                                                                         |


## <a name="response"></a><span data-ttu-id="8672e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8672e-144">Response</span></span>

<span data-ttu-id="8672e-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект коллекции [информатионпротектионактион](../resources/informationprotectionaction.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8672e-145">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="8672e-146">[Объект информатионпротектионактион](../resources/informationprotectionaction.md) будет содержать объект [метадатаактион](../resources/metadataaction.md) , который информирует приложение о том, какие метаданные необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="8672e-146">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="8672e-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="8672e-147">Examples</span></span>

<span data-ttu-id="8672e-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8672e-148">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8672e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="8672e-149">Request</span></span>

<span data-ttu-id="8672e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8672e-150">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8672e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8672e-151">Response</span></span>

<span data-ttu-id="8672e-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8672e-152">The following is an example of the response.</span></span>

> <span data-ttu-id="8672e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8672e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
