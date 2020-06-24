---
title: Создание Коннекторграуп
description: Создание объекта Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ddc1aebfeb64e4dd596f94dd8a91f3718a29fb7
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863274"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="5e075-103">Создание Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="5e075-103">Create connectorGroup</span></span>

<span data-ttu-id="5e075-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e075-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e075-105">Создание объекта [коннекторграуп](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="5e075-105">Create a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e075-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e075-106">Permissions</span></span>
<span data-ttu-id="5e075-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5e075-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5e075-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e075-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e075-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e075-109">Permission type</span></span>      | <span data-ttu-id="5e075-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e075-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e075-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e075-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e075-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e075-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e075-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e075-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e075-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e075-114">Not supported.</span></span>    |
|<span data-ttu-id="5e075-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e075-115">Application</span></span> | <span data-ttu-id="5e075-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e075-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5e075-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e075-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-request-headers"></a><span data-ttu-id="5e075-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e075-118">Optional request headers</span></span>
| <span data-ttu-id="5e075-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5e075-119">Name</span></span>       | <span data-ttu-id="5e075-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5e075-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5e075-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e075-121">Authorization</span></span>  | <span data-ttu-id="5e075-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="5e075-122">Bearer.</span></span> <span data-ttu-id="5e075-123">Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="5e075-123">Required.</span></span>|
| <span data-ttu-id="5e075-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e075-124">Content-type</span></span> | <span data-ttu-id="5e075-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="5e075-125">application/json.</span></span> <span data-ttu-id="5e075-126">Required.</span><span class="sxs-lookup"><span data-stu-id="5e075-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e075-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e075-127">Request body</span></span>
<span data-ttu-id="5e075-128">В тексте запроса добавьте представление объекта [коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e075-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>
<span data-ttu-id="5e075-129">В следующей таблице перечислены свойства, доступные для **коннекторграуп**.</span><span class="sxs-lookup"><span data-stu-id="5e075-129">The following table lists the properties available for a **connectorGroup**.</span></span> <span data-ttu-id="5e075-130">Свойство **Name** — это обязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="5e075-130">The **name** property is a required property.</span></span>

| <span data-ttu-id="5e075-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e075-131">Property</span></span>     | <span data-ttu-id="5e075-132">Тип</span><span class="sxs-lookup"><span data-stu-id="5e075-132">Type</span></span>   |<span data-ttu-id="5e075-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5e075-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e075-134">коннекторграуптипе</span><span class="sxs-lookup"><span data-stu-id="5e075-134">connectorGroupType</span></span>|<span data-ttu-id="5e075-135">string</span><span class="sxs-lookup"><span data-stu-id="5e075-135">string</span></span>| <span data-ttu-id="5e075-136">Указывает тип гибридного агента.</span><span class="sxs-lookup"><span data-stu-id="5e075-136">Indicates the type of hybrid agent.</span></span> <span data-ttu-id="5e075-137">Это свойство предустановлено системой.</span><span class="sxs-lookup"><span data-stu-id="5e075-137">This property is preset by the system.</span></span>|
|<span data-ttu-id="5e075-138">id</span><span class="sxs-lookup"><span data-stu-id="5e075-138">id</span></span>|<span data-ttu-id="5e075-139">строка</span><span class="sxs-lookup"><span data-stu-id="5e075-139">string</span></span>| <span data-ttu-id="5e075-140">Уникальный идентификатор для этого Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5e075-140">Unique identifier for this connectorGroup.</span></span> <span data-ttu-id="5e075-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e075-141">Read-only.</span></span> |
|<span data-ttu-id="5e075-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="5e075-142">isDefault</span></span>|<span data-ttu-id="5e075-143">boolean</span><span class="sxs-lookup"><span data-stu-id="5e075-143">boolean</span></span>| <span data-ttu-id="5e075-144">Указывает, является ли Коннекторграуп значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5e075-144">Indicates whether the connectorGroup is the default.</span></span> <span data-ttu-id="5e075-145">Только одна группа соединителей может быть Коннекторграуп по умолчанию, и она предустановлена системой.</span><span class="sxs-lookup"><span data-stu-id="5e075-145">Only a single connector group can be the default connectorGroup and this is preset by the system.</span></span> |
|<span data-ttu-id="5e075-146">name</span><span class="sxs-lookup"><span data-stu-id="5e075-146">name</span></span>|<span data-ttu-id="5e075-147">string</span><span class="sxs-lookup"><span data-stu-id="5e075-147">string</span></span>| <span data-ttu-id="5e075-148">Имя, связанное с Коннекторграуп.</span><span class="sxs-lookup"><span data-stu-id="5e075-148">The name associated with the connectorGroup.</span></span> |
|<span data-ttu-id="5e075-149">региональных</span><span class="sxs-lookup"><span data-stu-id="5e075-149">region</span></span>|<span data-ttu-id="5e075-150">string</span><span class="sxs-lookup"><span data-stu-id="5e075-150">string</span></span>| <span data-ttu-id="5e075-151">Регион, которому назначена Коннекторграуп, и который оптимизирует трафик для.</span><span class="sxs-lookup"><span data-stu-id="5e075-151">The region the connectorGroup is assigned to and will optimize traffic for.</span></span> <span data-ttu-id="5e075-152">Эту область можно задать только в том случае, если Коннекторграуп **не назначен ни один** из соединителей или приложений.</span><span class="sxs-lookup"><span data-stu-id="5e075-152">This region can only be set if **no** connectors or applications are assigned to the connectorGroup.</span></span> <span data-ttu-id="5e075-153">Доступны следующие регионы: Северная Америка, Европа, Австралия, Азия и Индии.</span><span class="sxs-lookup"><span data-stu-id="5e075-153">The regions available include: North America, Europe, Australia, Asia, and India.</span></span> <span data-ttu-id="5e075-154">Возможные значения: `nam`, `eur`, `aus`, `asia`, `ind`.</span><span class="sxs-lookup"><span data-stu-id="5e075-154">Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`.</span></span>|

## <a name="response"></a><span data-ttu-id="5e075-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e075-155">Response</span></span>

<span data-ttu-id="5e075-156">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e075-156">If successful, this method returns a `201 Created` response code and a [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e075-157">Пример</span><span class="sxs-lookup"><span data-stu-id="5e075-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e075-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e075-158">Request</span></span>
<span data-ttu-id="5e075-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e075-159">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "Connector Group Demo"

}
```
### <a name="response"></a><span data-ttu-id="5e075-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e075-160">Response</span></span>
<span data-ttu-id="5e075-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e075-161">The following is an example of the response.</span></span> 

><span data-ttu-id="5e075-162">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5e075-162">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5e075-163">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5e075-163">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
  "name": "Connector Group Demo",
  "connectorGroupType": "applicationProxy",
  "isDefault": true,
  "region": "nam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
