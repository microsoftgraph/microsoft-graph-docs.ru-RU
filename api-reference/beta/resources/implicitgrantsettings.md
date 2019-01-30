---
title: Тип ресурса implicitGrantSettings
description: Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения. Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока. Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642767"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="a85bc-105">Тип ресурса implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="a85bc-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a85bc-106">Разрешение запроса маркеры, с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a85bc-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="a85bc-107">Отдельные свойства доступны для запроса маркеры идентификатор и доступа как часть неявных потока.</span><span class="sxs-lookup"><span data-stu-id="a85bc-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="a85bc-108">Чтобы включить неявных поток, по крайней мере одного из следующих свойств необходимо установить значение true.</span><span class="sxs-lookup"><span data-stu-id="a85bc-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="a85bc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a85bc-109">Properties</span></span>

| <span data-ttu-id="a85bc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a85bc-110">Property</span></span> | <span data-ttu-id="a85bc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a85bc-111">Type</span></span> | <span data-ttu-id="a85bc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a85bc-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="a85bc-113">enableIdTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="a85bc-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="a85bc-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a85bc-114">Boolean</span></span> | <span data-ttu-id="a85bc-115">Разрешение запроса с помощью поток неявных OAuth 2.0 маркера Идентификации данного веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a85bc-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="a85bc-116">enableAccessTokenIssuance</span><span class="sxs-lookup"><span data-stu-id="a85bc-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="a85bc-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a85bc-117">Boolean</span></span> | <span data-ttu-id="a85bc-118">Разрешение запроса маркер доступа с помощью поток неявных OAuth 2.0 этого веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="a85bc-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a85bc-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a85bc-119">JSON representation</span></span>
<span data-ttu-id="a85bc-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a85bc-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
