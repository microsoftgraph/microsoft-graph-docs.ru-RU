---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74c480b8117f3d8dbf0ad8208bac09b63b113906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156191"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="840d9-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="840d9-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="840d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="840d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="840d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="840d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="840d9-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="840d9-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="840d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="840d9-107">Properties</span></span>
|<span data-ttu-id="840d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="840d9-108">Property</span></span>|<span data-ttu-id="840d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="840d9-109">Type</span></span>|<span data-ttu-id="840d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="840d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="840d9-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="840d9-111">subjectName</span></span>|<span data-ttu-id="840d9-112">String</span><span class="sxs-lookup"><span data-stu-id="840d9-112">String</span></span>|<span data-ttu-id="840d9-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="840d9-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="840d9-114">description</span><span class="sxs-lookup"><span data-stu-id="840d9-114">description</span></span>|<span data-ttu-id="840d9-115">String</span><span class="sxs-lookup"><span data-stu-id="840d9-115">String</span></span>|<span data-ttu-id="840d9-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="840d9-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="840d9-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="840d9-117">expirationDateTime</span></span>|<span data-ttu-id="840d9-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="840d9-118">DateTimeOffset</span></span>|<span data-ttu-id="840d9-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="840d9-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="840d9-120">certificate</span><span class="sxs-lookup"><span data-stu-id="840d9-120">certificate</span></span>|<span data-ttu-id="840d9-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="840d9-121">Binary</span></span>|<span data-ttu-id="840d9-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="840d9-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="840d9-123">Связи</span><span class="sxs-lookup"><span data-stu-id="840d9-123">Relationships</span></span>
<span data-ttu-id="840d9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="840d9-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="840d9-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="840d9-125">JSON Representation</span></span>
<span data-ttu-id="840d9-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="840d9-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```




