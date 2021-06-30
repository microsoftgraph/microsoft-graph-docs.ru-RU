---
title: тип ресурса cloudPcUserRoleScopeTagInfo
description: Представляет сведения тега области с отображаемой именем и удостоверением.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61df383dca51ec2494eb10b745bc227bcfc5d9b8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211310"
---
# <a name="cloudpcuserrolescopetaginfo-resource-type"></a><span data-ttu-id="32521-103">тип ресурса cloudPcUserRoleScopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="32521-103">cloudPcUserRoleScopeTagInfo resource type</span></span>

<span data-ttu-id="32521-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32521-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32521-105">Представляет сведения тега области с отображаемой именем и удостоверением.</span><span class="sxs-lookup"><span data-stu-id="32521-105">Represents the scope tag info with display name and identity.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="32521-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="32521-106">Properties</span></span>
|<span data-ttu-id="32521-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="32521-107">Property</span></span>|<span data-ttu-id="32521-108">Тип</span><span class="sxs-lookup"><span data-stu-id="32521-108">Type</span></span>|<span data-ttu-id="32521-109">Описание</span><span class="sxs-lookup"><span data-stu-id="32521-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32521-110">displayName</span><span class="sxs-lookup"><span data-stu-id="32521-110">displayName</span></span>|<span data-ttu-id="32521-111">String</span><span class="sxs-lookup"><span data-stu-id="32521-111">String</span></span>|<span data-ttu-id="32521-112">Имя отображения тегов области.</span><span class="sxs-lookup"><span data-stu-id="32521-112">Scope tag display name.</span></span>|
|<span data-ttu-id="32521-113">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="32521-113">roleScopeTagId</span></span>|<span data-ttu-id="32521-114">String</span><span class="sxs-lookup"><span data-stu-id="32521-114">String</span></span>|<span data-ttu-id="32521-115">ID тега области.</span><span class="sxs-lookup"><span data-stu-id="32521-115">Scope tag ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32521-116">Связи</span><span class="sxs-lookup"><span data-stu-id="32521-116">Relationships</span></span>

<span data-ttu-id="32521-117">Нет</span><span class="sxs-lookup"><span data-stu-id="32521-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32521-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32521-118">JSON Representation</span></span>
<span data-ttu-id="32521-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32521-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserRoleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```