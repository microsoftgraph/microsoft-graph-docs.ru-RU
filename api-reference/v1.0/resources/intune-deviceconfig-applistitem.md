---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c0e880b8afebdfccab426fbe80966cc3f828a19
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755926"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="b414b-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="b414b-103">appListItem resource type</span></span>

<span data-ttu-id="b414b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b414b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b414b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b414b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b414b-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="b414b-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="b414b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b414b-107">Properties</span></span>
|<span data-ttu-id="b414b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b414b-108">Property</span></span>|<span data-ttu-id="b414b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b414b-109">Type</span></span>|<span data-ttu-id="b414b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b414b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b414b-111">name</span><span class="sxs-lookup"><span data-stu-id="b414b-111">name</span></span>|<span data-ttu-id="b414b-112">String</span><span class="sxs-lookup"><span data-stu-id="b414b-112">String</span></span>|<span data-ttu-id="b414b-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="b414b-113">The application name</span></span>|
|<span data-ttu-id="b414b-114">publisher</span><span class="sxs-lookup"><span data-stu-id="b414b-114">publisher</span></span>|<span data-ttu-id="b414b-115">String</span><span class="sxs-lookup"><span data-stu-id="b414b-115">String</span></span>|<span data-ttu-id="b414b-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="b414b-116">The publisher of the application</span></span>|
|<span data-ttu-id="b414b-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b414b-117">appStoreUrl</span></span>|<span data-ttu-id="b414b-118">String</span><span class="sxs-lookup"><span data-stu-id="b414b-118">String</span></span>|<span data-ttu-id="b414b-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="b414b-119">The Store URL of the application</span></span>|
|<span data-ttu-id="b414b-120">appId</span><span class="sxs-lookup"><span data-stu-id="b414b-120">appId</span></span>|<span data-ttu-id="b414b-121">String</span><span class="sxs-lookup"><span data-stu-id="b414b-121">String</span></span>|<span data-ttu-id="b414b-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="b414b-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="b414b-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="b414b-123">Relationships</span></span>
<span data-ttu-id="b414b-124">Нет</span><span class="sxs-lookup"><span data-stu-id="b414b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b414b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b414b-125">JSON Representation</span></span>
<span data-ttu-id="b414b-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b414b-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




