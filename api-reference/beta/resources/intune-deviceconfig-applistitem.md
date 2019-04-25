---
title: Тип ресурса appListItem
description: Представляет приложение в списке управляемых приложений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f452de7d002368c204cb57cc352ac9f9658609a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549561"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="d7db7-103">Тип ресурса appListItem</span><span class="sxs-lookup"><span data-stu-id="d7db7-103">appListItem resource type</span></span>

> <span data-ttu-id="d7db7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7db7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7db7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7db7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7db7-106">Представляет приложение в списке управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="d7db7-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="d7db7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7db7-107">Properties</span></span>
|<span data-ttu-id="d7db7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7db7-108">Property</span></span>|<span data-ttu-id="d7db7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d7db7-109">Type</span></span>|<span data-ttu-id="d7db7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d7db7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7db7-111">name</span><span class="sxs-lookup"><span data-stu-id="d7db7-111">name</span></span>|<span data-ttu-id="d7db7-112">String</span><span class="sxs-lookup"><span data-stu-id="d7db7-112">String</span></span>|<span data-ttu-id="d7db7-113">Имя приложения</span><span class="sxs-lookup"><span data-stu-id="d7db7-113">The application name</span></span>|
|<span data-ttu-id="d7db7-114">publisher</span><span class="sxs-lookup"><span data-stu-id="d7db7-114">publisher</span></span>|<span data-ttu-id="d7db7-115">String</span><span class="sxs-lookup"><span data-stu-id="d7db7-115">String</span></span>|<span data-ttu-id="d7db7-116">Издатель приложения</span><span class="sxs-lookup"><span data-stu-id="d7db7-116">The publisher of the application</span></span>|
|<span data-ttu-id="d7db7-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d7db7-117">appStoreUrl</span></span>|<span data-ttu-id="d7db7-118">String</span><span class="sxs-lookup"><span data-stu-id="d7db7-118">String</span></span>|<span data-ttu-id="d7db7-119">URL-адрес приложения в Магазине</span><span class="sxs-lookup"><span data-stu-id="d7db7-119">The Store URL of the application</span></span>|
|<span data-ttu-id="d7db7-120">appId</span><span class="sxs-lookup"><span data-stu-id="d7db7-120">appId</span></span>|<span data-ttu-id="d7db7-121">String</span><span class="sxs-lookup"><span data-stu-id="d7db7-121">String</span></span>|<span data-ttu-id="d7db7-122">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="d7db7-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7db7-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="d7db7-123">Relationships</span></span>
<span data-ttu-id="d7db7-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d7db7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7db7-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7db7-125">JSON Representation</span></span>
<span data-ttu-id="d7db7-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7db7-126">Here is a JSON representation of the resource.</span></span>
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





