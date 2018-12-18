---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
ms.openlocfilehash: a66c1eeae6d405aa8d0546ac0143e2a8b3404231
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361665"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="8c6b5-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="8c6b5-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="8c6b5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c6b5-105">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="8c6b5-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="8c6b5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c6b5-106">Properties</span></span>
|<span data-ttu-id="8c6b5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c6b5-107">Property</span></span>|<span data-ttu-id="8c6b5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8c6b5-108">Type</span></span>|<span data-ttu-id="8c6b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8c6b5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c6b5-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="8c6b5-110">subjectName</span></span>|<span data-ttu-id="8c6b5-111">String</span><span class="sxs-lookup"><span data-stu-id="8c6b5-111">String</span></span>|<span data-ttu-id="8c6b5-112">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8c6b5-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="8c6b5-113">описание</span><span class="sxs-lookup"><span data-stu-id="8c6b5-113">description</span></span>|<span data-ttu-id="8c6b5-114">String</span><span class="sxs-lookup"><span data-stu-id="8c6b5-114">String</span></span>|<span data-ttu-id="8c6b5-115">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8c6b5-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="8c6b5-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8c6b5-116">expirationDateTime</span></span>|<span data-ttu-id="8c6b5-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c6b5-117">DateTimeOffset</span></span>|<span data-ttu-id="8c6b5-118">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8c6b5-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="8c6b5-119">certificate</span><span class="sxs-lookup"><span data-stu-id="8c6b5-119">certificate</span></span>|<span data-ttu-id="8c6b5-120">Двоичный</span><span class="sxs-lookup"><span data-stu-id="8c6b5-120">Binary</span></span>|<span data-ttu-id="8c6b5-121">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="8c6b5-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c6b5-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8c6b5-122">Relationships</span></span>
<span data-ttu-id="8c6b5-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8c6b5-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c6b5-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c6b5-124">JSON Representation</span></span>
<span data-ttu-id="8c6b5-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c6b5-125">Here is a JSON representation of the resource.</span></span>
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



