---
title: Тип ресурса Виндовскиосказуреадграуп
description: Класс, используемый для идентификации группы AzureAD для конфигурации киоска
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f05bf9d01e8442a54c9fa70b863e3789309bd9d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175138"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="ea283-103">Тип ресурса Виндовскиосказуреадграуп</span><span class="sxs-lookup"><span data-stu-id="ea283-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="ea283-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea283-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea283-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea283-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea283-106">Класс, используемый для идентификации группы AzureAD для конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="ea283-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="ea283-107">НаСледуется от [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="ea283-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea283-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea283-108">Properties</span></span>
|<span data-ttu-id="ea283-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea283-109">Property</span></span>|<span data-ttu-id="ea283-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea283-110">Type</span></span>|<span data-ttu-id="ea283-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea283-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea283-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ea283-112">displayName</span></span>|<span data-ttu-id="ea283-113">String</span><span class="sxs-lookup"><span data-stu-id="ea283-113">String</span></span>|<span data-ttu-id="ea283-114">Отображаемое имя группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="ea283-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="ea283-115">groupId</span><span class="sxs-lookup"><span data-stu-id="ea283-115">groupId</span></span>|<span data-ttu-id="ea283-116">String</span><span class="sxs-lookup"><span data-stu-id="ea283-116">String</span></span>|<span data-ttu-id="ea283-117">Идентификатор группы AzureAD, которая будет заблокирована для этой конфигурации киоска</span><span class="sxs-lookup"><span data-stu-id="ea283-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea283-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="ea283-118">Relationships</span></span>
<span data-ttu-id="ea283-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ea283-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea283-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea283-120">JSON Representation</span></span>
<span data-ttu-id="ea283-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea283-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```




