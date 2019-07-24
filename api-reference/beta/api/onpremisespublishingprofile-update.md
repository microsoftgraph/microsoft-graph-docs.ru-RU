---
title: Обновление Онпремисеспублишингпрофиле
description: Обновление свойств объекта Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c2cdd2eafc51e5bd38aed41fcfcae259b5a9fe66
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841082"
---
# <a name="update-onpremisespublishingprofile"></a><span data-ttu-id="9a497-103">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="9a497-103">Update onPremisesPublishingProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a497-104">Обновление свойств объекта [онпремисеспублишингпрофиле](../resources/onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="9a497-104">Update the properties of an [onPremisesPublishingProfile](../resources/onpremisespublishingprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a497-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a497-105">Permissions</span></span>

<span data-ttu-id="9a497-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a497-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a497-108">Permission type</span></span>                        | <span data-ttu-id="9a497-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a497-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="9a497-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a497-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a497-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9a497-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="9a497-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a497-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a497-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a497-113">Not supported.</span></span> |
| <span data-ttu-id="9a497-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a497-114">Application</span></span>                            | <span data-ttu-id="9a497-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a497-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a497-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a497-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/hybridAgentUpdaterConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="9a497-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a497-117">Request headers</span></span>

| <span data-ttu-id="9a497-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9a497-118">Name</span></span>       | <span data-ttu-id="9a497-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9a497-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9a497-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a497-120">Authorization</span></span> | <span data-ttu-id="9a497-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9a497-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a497-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a497-122">Request body</span></span>

<span data-ttu-id="9a497-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9a497-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="9a497-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9a497-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9a497-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9a497-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9a497-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a497-126">Property</span></span>     | <span data-ttu-id="9a497-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9a497-127">Type</span></span>        | <span data-ttu-id="9a497-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9a497-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a497-129">Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9a497-129">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="9a497-130">Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9a497-130">hybridAgentUpdaterConfiguration</span></span>|<span data-ttu-id="9a497-131">Представляет [хибридажентупдатерконфигуратион](../resources/hybridagentupdaterconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9a497-131">Represents [hybridAgentUpdaterConfiguration](../resources/hybridagentupdaterconfiguration.md).</span></span>|

## <a name="response"></a><span data-ttu-id="9a497-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a497-132">Response</span></span>

<span data-ttu-id="9a497-133">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9a497-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9a497-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a497-134">Examples</span></span>

### <a name="example-1-update-updatewindow-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="9a497-135">Пример 1: обновление Упдатевиндов в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9a497-135">Example 1: Update updateWindow in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="9a497-136">В следующем примере выполняется обновление **упдатевиндов** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="9a497-136">The following example updates the **updateWindow** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="9a497-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a497-137">Request</span></span>

<span data-ttu-id="9a497-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a497-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
   "updateWindow" :
{
      "updateWindowStartTime" : "0:00:00",
      "updateWindowEndTime" : "23:59:00"
  }
}
```

#### <a name="response"></a><span data-ttu-id="9a497-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a497-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-deferupdate-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="9a497-140">Пример 2: обновление Деферупдате в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9a497-140">Example 2: Update deferUpdate in the hybridAgentUpdaterConfiguration</span></span> 

<span data-ttu-id="9a497-141">В следующем примере показано, как обновить **деферупдате** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="9a497-141">The following example updates **deferUpdate** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="9a497-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a497-142">Request</span></span>

<span data-ttu-id="9a497-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a497-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "deferUpdate" : "2018-08-20T12:00"
}
```

#### <a name="response"></a><span data-ttu-id="9a497-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a497-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-allowupdateconfigurationoverride-in-the-hybridagentupdaterconfiguration"></a><span data-ttu-id="9a497-145">Пример 3: обновление Алловупдатеконфигуратионоверриде в Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9a497-145">Example 3: Update allowUpdateConfigurationOverride in the hybridAgentUpdaterConfiguration</span></span>

<span data-ttu-id="9a497-146">В следующем примере показано, как обновить **алловупдатеконфигуратионоверриде** в **хибридажентупдатерконфигуратион**.</span><span class="sxs-lookup"><span data-stu-id="9a497-146">The following example updates **allowUpdateConfigurationOverride** in the **hybridAgentUpdaterConfiguration**.</span></span>

#### <a name="request"></a><span data-ttu-id="9a497-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a497-147">Request</span></span>

<span data-ttu-id="9a497-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a497-148">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_onpremisespublishingprofile"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration
Content-Type: application/json

{
    "allowUpdateConfigurationOverride" : false
}
```

#### <a name="response"></a><span data-ttu-id="9a497-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a497-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisespublishingprofile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
