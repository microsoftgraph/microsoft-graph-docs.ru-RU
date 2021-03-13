---
title: тип ресурса connectionInfo
description: Объект connectionInfo определяет сведения о подключении, используемые для связи с ресурсом.
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8bbab1e93cf5af0fcfbd401b6b726f3165f595b4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761823"
---
# <a name="connectioninfo-resource-type"></a><span data-ttu-id="f857e-103">тип ресурса connectionInfo</span><span class="sxs-lookup"><span data-stu-id="f857e-103">connectionInfo resource type</span></span>

<span data-ttu-id="f857e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f857e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f857e-105">Объект connectionInfo определяет локатор ресурсов, используемый для связи с ресурсом в Azure AD Entitlement Management.</span><span class="sxs-lookup"><span data-stu-id="f857e-105">The connectionInfo object defines the resource locator that is used to communicate with a resource in Azure AD Entitlement Management.</span></span>

## <a name="properties"></a><span data-ttu-id="f857e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f857e-106">Properties</span></span>
|<span data-ttu-id="f857e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f857e-107">Property</span></span>|<span data-ttu-id="f857e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f857e-108">Type</span></span>|<span data-ttu-id="f857e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f857e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f857e-110">url</span><span class="sxs-lookup"><span data-stu-id="f857e-110">url</span></span>|<span data-ttu-id="f857e-111">String</span><span class="sxs-lookup"><span data-stu-id="f857e-111">String</span></span>|<span data-ttu-id="f857e-112">Конечная точка, используемая управлением правами для связи с ресурсом пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="f857e-112">The endpoint that is used by Entitlement Management to communicate with the access package resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f857e-113">Отношения</span><span class="sxs-lookup"><span data-stu-id="f857e-113">Relationships</span></span>
<span data-ttu-id="f857e-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f857e-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f857e-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f857e-115">JSON representation</span></span>
<span data-ttu-id="f857e-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f857e-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionInfo",
  "url": "String"
}
```
