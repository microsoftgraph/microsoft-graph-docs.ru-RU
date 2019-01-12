---
title: Тип ресурса windowsInformationProtectionDataRecoveryCertificate
description: Сертификат восстановления данных Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5e686ab1a6c1e586c8bd32c56d3480102503b4be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976256"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="fb962-103">Тип ресурса windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="fb962-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="fb962-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb962-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb962-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb962-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb962-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb962-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb962-107">Сертификат восстановления данных Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fb962-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="fb962-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb962-108">Properties</span></span>
|<span data-ttu-id="fb962-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb962-109">Property</span></span>|<span data-ttu-id="fb962-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fb962-110">Type</span></span>|<span data-ttu-id="fb962-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fb962-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb962-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="fb962-112">subjectName</span></span>|<span data-ttu-id="fb962-113">String</span><span class="sxs-lookup"><span data-stu-id="fb962-113">String</span></span>|<span data-ttu-id="fb962-114">Имя субъекта для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="fb962-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="fb962-115">описание</span><span class="sxs-lookup"><span data-stu-id="fb962-115">description</span></span>|<span data-ttu-id="fb962-116">String</span><span class="sxs-lookup"><span data-stu-id="fb962-116">String</span></span>|<span data-ttu-id="fb962-117">Описание сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="fb962-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="fb962-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fb962-118">expirationDateTime</span></span>|<span data-ttu-id="fb962-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb962-119">DateTimeOffset</span></span>|<span data-ttu-id="fb962-120">Дата и время окончания срока действия для сертификата восстановления данных</span><span class="sxs-lookup"><span data-stu-id="fb962-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="fb962-121">certificate</span><span class="sxs-lookup"><span data-stu-id="fb962-121">certificate</span></span>|<span data-ttu-id="fb962-122">Двоичный</span><span class="sxs-lookup"><span data-stu-id="fb962-122">Binary</span></span>|<span data-ttu-id="fb962-123">Сертификат восстановления данных</span><span class="sxs-lookup"><span data-stu-id="fb962-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb962-124">Связи</span><span class="sxs-lookup"><span data-stu-id="fb962-124">Relationships</span></span>
<span data-ttu-id="fb962-125">Нет</span><span class="sxs-lookup"><span data-stu-id="fb962-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fb962-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb962-126">JSON Representation</span></span>
<span data-ttu-id="fb962-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb962-127">Here is a JSON representation of the resource.</span></span>
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





