---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fce6d146e267d0b64d1f95cf15e23b92e6e33720
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468430"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="a80e0-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a80e0-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="a80e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a80e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a80e0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a80e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a80e0-106">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="a80e0-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="a80e0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a80e0-107">Properties</span></span>
|<span data-ttu-id="a80e0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a80e0-108">Property</span></span>|<span data-ttu-id="a80e0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a80e0-109">Type</span></span>|<span data-ttu-id="a80e0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a80e0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a80e0-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="a80e0-111">subjectName</span></span>|<span data-ttu-id="a80e0-112">String</span><span class="sxs-lookup"><span data-stu-id="a80e0-112">String</span></span>|<span data-ttu-id="a80e0-113">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a80e0-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="a80e0-114">description</span><span class="sxs-lookup"><span data-stu-id="a80e0-114">description</span></span>|<span data-ttu-id="a80e0-115">String</span><span class="sxs-lookup"><span data-stu-id="a80e0-115">String</span></span>|<span data-ttu-id="a80e0-116">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a80e0-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="a80e0-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a80e0-117">expirationDateTime</span></span>|<span data-ttu-id="a80e0-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a80e0-118">DateTimeOffset</span></span>|<span data-ttu-id="a80e0-119">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a80e0-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="a80e0-120">certificate</span><span class="sxs-lookup"><span data-stu-id="a80e0-120">certificate</span></span>|<span data-ttu-id="a80e0-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a80e0-121">Binary</span></span>|<span data-ttu-id="a80e0-122">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="a80e0-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a80e0-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="a80e0-123">Relationships</span></span>
<span data-ttu-id="a80e0-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a80e0-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a80e0-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a80e0-125">JSON Representation</span></span>
<span data-ttu-id="a80e0-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a80e0-126">Here is a JSON representation of the resource.</span></span>
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







