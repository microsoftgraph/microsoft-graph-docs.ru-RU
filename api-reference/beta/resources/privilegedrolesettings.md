---
title: Тип ресурса Привилежедролесеттингс
description: Представляет параметры привилегированной роли.
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563287"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="4e752-103">Тип ресурса Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="4e752-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e752-104">Представляет параметры привилегированной роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="4e752-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4e752-105">Methods</span></span>

| <span data-ttu-id="4e752-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4e752-106">Method</span></span>           | <span data-ttu-id="4e752-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e752-107">Return Type</span></span>    |<span data-ttu-id="4e752-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4e752-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e752-109">Получение privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="4e752-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="4e752-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="4e752-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="4e752-111">Чтение свойств и связей объекта Привилежедролесеттингс.</span><span class="sxs-lookup"><span data-stu-id="4e752-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="4e752-112">Обновление Привилежедролесеттингс</span><span class="sxs-lookup"><span data-stu-id="4e752-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="4e752-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="4e752-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="4e752-114">Обновление объекта Привилежедролесеттингс.</span><span class="sxs-lookup"><span data-stu-id="4e752-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="4e752-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e752-115">Properties</span></span>
| <span data-ttu-id="4e752-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e752-116">Property</span></span>     | <span data-ttu-id="4e752-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4e752-117">Type</span></span>   |<span data-ttu-id="4e752-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4e752-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e752-119">Елеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="4e752-119">elevationDuration</span></span>|<span data-ttu-id="4e752-120">duration</span><span class="sxs-lookup"><span data-stu-id="4e752-120">duration</span></span>|<span data-ttu-id="4e752-121">Продолжительность активации роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="4e752-122">id</span><span class="sxs-lookup"><span data-stu-id="4e752-122">id</span></span>|<span data-ttu-id="4e752-123">string</span><span class="sxs-lookup"><span data-stu-id="4e752-123">string</span></span>| <span data-ttu-id="4e752-124">Уникальный идентификатор для параметров роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="4e752-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e752-125">Read-only.</span></span>|
|<span data-ttu-id="4e752-126">Исмфаонелеватионконфигурабле</span><span class="sxs-lookup"><span data-stu-id="4e752-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="4e752-127">boolean</span><span class="sxs-lookup"><span data-stu-id="4e752-127">boolean</span></span>|<span data-ttu-id="4e752-128">**значение true** , если мфаонелеватион является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="4e752-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="4e752-129">**false** , если мфаонелеватион не является настраиваемым.</span><span class="sxs-lookup"><span data-stu-id="4e752-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="4e752-130">Ластглобаладмин</span><span class="sxs-lookup"><span data-stu-id="4e752-130">lastGlobalAdmin</span></span>|<span data-ttu-id="4e752-131">boolean</span><span class="sxs-lookup"><span data-stu-id="4e752-131">boolean</span></span>|<span data-ttu-id="4e752-132">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="4e752-132">Internal used only.</span></span>|
|<span data-ttu-id="4e752-133">Макселаватиондуратион</span><span class="sxs-lookup"><span data-stu-id="4e752-133">maxElavationDuration</span></span>|<span data-ttu-id="4e752-134">duration</span><span class="sxs-lookup"><span data-stu-id="4e752-134">duration</span></span>|<span data-ttu-id="4e752-135">Максимальный срок для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="4e752-136">Мфаонелеватион</span><span class="sxs-lookup"><span data-stu-id="4e752-136">mfaOnElevation</span></span>|<span data-ttu-id="4e752-137">boolean</span><span class="sxs-lookup"><span data-stu-id="4e752-137">boolean</span></span>|<span data-ttu-id="4e752-138">**значение true** , если для активации роли требуется mfa.</span><span class="sxs-lookup"><span data-stu-id="4e752-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="4e752-139">**false** , если MFA не требуется для активации роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="4e752-140">Минелеватиондуратион</span><span class="sxs-lookup"><span data-stu-id="4e752-140">minElevationDuration</span></span>|<span data-ttu-id="4e752-141">duration</span><span class="sxs-lookup"><span data-stu-id="4e752-141">duration</span></span>|<span data-ttu-id="4e752-142">Минимальная длительность для активированной роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="4e752-143">Нотификатионтаусеронелеватион</span><span class="sxs-lookup"><span data-stu-id="4e752-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="4e752-144">boolean</span><span class="sxs-lookup"><span data-stu-id="4e752-144">boolean</span></span>|<span data-ttu-id="4e752-145">**имеет значение true** , если вы отправляете уведомление конечному пользователю при активации роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="4e752-146">**значение false** , если уведомление не отправляется при активации роли.</span><span class="sxs-lookup"><span data-stu-id="4e752-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="4e752-147">Тиккетингинфунелеватион</span><span class="sxs-lookup"><span data-stu-id="4e752-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="4e752-148">boolean</span><span class="sxs-lookup"><span data-stu-id="4e752-148">boolean</span></span>|<span data-ttu-id="4e752-149">**имеет значение true** , если при активации роли требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="4e752-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="4e752-150">**false** , если при активации роли не требуются сведения о билетах.</span><span class="sxs-lookup"><span data-stu-id="4e752-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="4e752-151">Аппровалонелеватион</span><span class="sxs-lookup"><span data-stu-id="4e752-151">approvalOnElevation</span></span>|<span data-ttu-id="4e752-152">boolean</span><span class="sxs-lookup"><span data-stu-id="4e752-152">boolean</span></span>|<span data-ttu-id="4e752-153">**имеет значение true** , если при активации роли необходимо выполнить утверждение.</span><span class="sxs-lookup"><span data-stu-id="4e752-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="4e752-154">**false** , если при активации роли не нужно утверждать.</span><span class="sxs-lookup"><span data-stu-id="4e752-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="4e752-155">Аппроверидс</span><span class="sxs-lookup"><span data-stu-id="4e752-155">approverIds</span></span>|<span data-ttu-id="4e752-156">массив</span><span class="sxs-lookup"><span data-stu-id="4e752-156">array</span></span>|<span data-ttu-id="4e752-157">Список идентификаторов утверждения, если для активации необходимо утверждение.</span><span class="sxs-lookup"><span data-stu-id="4e752-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e752-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="4e752-158">Relationships</span></span>
<span data-ttu-id="4e752-159">Нет</span><span class="sxs-lookup"><span data-stu-id="4e752-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4e752-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e752-160">JSON representation</span></span>

<span data-ttu-id="4e752-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e752-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": []
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
