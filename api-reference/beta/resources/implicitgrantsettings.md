---
title: Тип ресурса ИмплиЦитгрантсеттингс
description: Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0. Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса. Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.
localization_priority: Normal
ms.openlocfilehash: 6714b9448f2e49419e41fa62822498ceaa232170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506228"
---
# <a name="implicitgrantsettings-resource-type"></a><span data-ttu-id="d3180-105">Тип ресурса ИмплиЦитгрантсеттингс</span><span class="sxs-lookup"><span data-stu-id="d3180-105">implicitGrantSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3180-106">Указывает, может ли это веб-приложение запрашивать маркеры, используя неявный поток OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="d3180-106">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span> <span data-ttu-id="d3180-107">Отдельные свойства доступны для идентификатора запроса и маркеров доступа в рамках неявного процесса.</span><span class="sxs-lookup"><span data-stu-id="d3180-107">Separate properties are available to request ID and access tokens as part of the implicit flow.</span></span> <span data-ttu-id="d3180-108">Чтобы разрешить неявный поток, по крайней мере одно из следующих свойств должно иметь значение true.</span><span class="sxs-lookup"><span data-stu-id="d3180-108">To enable implicit flow, at least one of the following properties must be set to true.</span></span>

## <a name="properties"></a><span data-ttu-id="d3180-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3180-109">Properties</span></span>

| <span data-ttu-id="d3180-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3180-110">Property</span></span> | <span data-ttu-id="d3180-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d3180-111">Type</span></span> | <span data-ttu-id="d3180-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d3180-112">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="d3180-113">Енаблеидтокениссуанце</span><span class="sxs-lookup"><span data-stu-id="d3180-113">enableIdTokenIssuance</span></span>| <span data-ttu-id="d3180-114">Логический</span><span class="sxs-lookup"><span data-stu-id="d3180-114">Boolean</span></span> | <span data-ttu-id="d3180-115">Указывает, может ли это веб-приложение запрашивать маркер идентификатора с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="d3180-115">Specifies whether this web application can request an ID token using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="d3180-116">Енаблеакцесстокениссуанце</span><span class="sxs-lookup"><span data-stu-id="d3180-116">enableAccessTokenIssuance</span></span>| <span data-ttu-id="d3180-117">Логический</span><span class="sxs-lookup"><span data-stu-id="d3180-117">Boolean</span></span> | <span data-ttu-id="d3180-118">Указывает, может ли это веб-приложение запрашивать маркер доступа с помощью неявного потока OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="d3180-118">Specifies whether this web application can request an access token using the OAuth 2.0 implicit flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3180-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3180-119">JSON representation</span></span>
<span data-ttu-id="d3180-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3180-120">Here is a JSON representation of the resource.</span></span>

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
