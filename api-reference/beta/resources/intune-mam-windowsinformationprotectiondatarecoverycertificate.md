---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32a18b25209301e3aeb62aaeaf63f080955cf669
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994533"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="d0f09-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="d0f09-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="d0f09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0f09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0f09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0f09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0f09-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="d0f09-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="d0f09-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0f09-107">Properties</span></span>
|<span data-ttu-id="d0f09-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0f09-108">Property</span></span>|<span data-ttu-id="d0f09-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0f09-109">Type</span></span>|<span data-ttu-id="d0f09-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0f09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0f09-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="d0f09-111">subjectName</span></span>|<span data-ttu-id="d0f09-112">String</span><span class="sxs-lookup"><span data-stu-id="d0f09-112">String</span></span>|<span data-ttu-id="d0f09-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d0f09-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="d0f09-114">description</span><span class="sxs-lookup"><span data-stu-id="d0f09-114">description</span></span>|<span data-ttu-id="d0f09-115">String</span><span class="sxs-lookup"><span data-stu-id="d0f09-115">String</span></span>|<span data-ttu-id="d0f09-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d0f09-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="d0f09-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f09-117">expirationDateTime</span></span>|<span data-ttu-id="d0f09-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f09-118">DateTimeOffset</span></span>|<span data-ttu-id="d0f09-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d0f09-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="d0f09-120">certificate</span><span class="sxs-lookup"><span data-stu-id="d0f09-120">certificate</span></span>|<span data-ttu-id="d0f09-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="d0f09-121">Binary</span></span>|<span data-ttu-id="d0f09-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="d0f09-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0f09-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="d0f09-123">Relationships</span></span>
<span data-ttu-id="d0f09-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d0f09-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0f09-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0f09-125">JSON Representation</span></span>
<span data-ttu-id="d0f09-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0f09-126">Here is a JSON representation of the resource.</span></span>
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





