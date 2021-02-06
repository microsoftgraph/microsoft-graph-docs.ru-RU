---
title: Тип ресурса connectionInfo
description: Объект connectionInfo определяет сведения о под соединении, используемые для связи с ресурсом.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dc7fcd045bb91819b39ad30f603191bab8380
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137736"
---
# <a name="connectioninfo-resource-type"></a><span data-ttu-id="06e3c-103">Тип ресурса connectionInfo</span><span class="sxs-lookup"><span data-stu-id="06e3c-103">connectionInfo resource type</span></span>

<span data-ttu-id="06e3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06e3c-105">Объект connectionInfo определяет локатор ресурсов, используемый для связи с ресурсом в azure AD Entitlement Management.</span><span class="sxs-lookup"><span data-stu-id="06e3c-105">The connectionInfo object defines the resource locator that is used to communicate with a resource in Azure AD Entitlement Management.</span></span>

## <a name="properties"></a><span data-ttu-id="06e3c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="06e3c-106">Properties</span></span>
|<span data-ttu-id="06e3c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="06e3c-107">Property</span></span>|<span data-ttu-id="06e3c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="06e3c-108">Type</span></span>|<span data-ttu-id="06e3c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="06e3c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e3c-110">url</span><span class="sxs-lookup"><span data-stu-id="06e3c-110">url</span></span>|<span data-ttu-id="06e3c-111">String</span><span class="sxs-lookup"><span data-stu-id="06e3c-111">String</span></span>|<span data-ttu-id="06e3c-112">Конечная точка, используемая управлением правами для связи с ресурсом пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="06e3c-112">The endpoint that is used by Entitlement Management to communicate with the access package resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06e3c-113">Связи</span><span class="sxs-lookup"><span data-stu-id="06e3c-113">Relationships</span></span>
<span data-ttu-id="06e3c-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="06e3c-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="06e3c-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="06e3c-115">JSON representation</span></span>
<span data-ttu-id="06e3c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06e3c-116">The following is a JSON representation of the resource.</span></span>
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
