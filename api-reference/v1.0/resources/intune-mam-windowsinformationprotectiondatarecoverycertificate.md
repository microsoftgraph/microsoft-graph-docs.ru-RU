---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
ms.openlocfilehash: 68faf0e78c68468216c3e69d64926f2c8b18e3c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027015"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="5f40e-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="5f40e-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="5f40e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5f40e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f40e-105">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="5f40e-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="5f40e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f40e-106">Properties</span></span>
|<span data-ttu-id="5f40e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f40e-107">Property</span></span>|<span data-ttu-id="5f40e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5f40e-108">Type</span></span>|<span data-ttu-id="5f40e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5f40e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f40e-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="5f40e-110">subjectName</span></span>|<span data-ttu-id="5f40e-111">String</span><span class="sxs-lookup"><span data-stu-id="5f40e-111">String</span></span>|<span data-ttu-id="5f40e-112">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="5f40e-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="5f40e-113">описание</span><span class="sxs-lookup"><span data-stu-id="5f40e-113">description</span></span>|<span data-ttu-id="5f40e-114">String</span><span class="sxs-lookup"><span data-stu-id="5f40e-114">String</span></span>|<span data-ttu-id="5f40e-115">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="5f40e-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="5f40e-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5f40e-116">expirationDateTime</span></span>|<span data-ttu-id="5f40e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f40e-117">DateTimeOffset</span></span>|<span data-ttu-id="5f40e-118">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="5f40e-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="5f40e-119">certificate</span><span class="sxs-lookup"><span data-stu-id="5f40e-119">certificate</span></span>|<span data-ttu-id="5f40e-120">Двоичный</span><span class="sxs-lookup"><span data-stu-id="5f40e-120">Binary</span></span>|<span data-ttu-id="5f40e-121">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="5f40e-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f40e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="5f40e-122">Relationships</span></span>
<span data-ttu-id="5f40e-123">Нет</span><span class="sxs-lookup"><span data-stu-id="5f40e-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f40e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f40e-124">JSON Representation</span></span>
<span data-ttu-id="5f40e-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f40e-125">Here is a JSON representation of the resource.</span></span>
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



