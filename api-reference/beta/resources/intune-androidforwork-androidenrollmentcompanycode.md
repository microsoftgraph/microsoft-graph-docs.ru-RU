---
title: Тип ресурса Андроиденроллменткомпаникоде
description: Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4271e788f51cc72a65b0343c229c502c940e0286
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021821"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="35704-103">Тип ресурса Андроиденроллменткомпаникоде</span><span class="sxs-lookup"><span data-stu-id="35704-103">androidEnrollmentCompanyCode resource type</span></span>

<span data-ttu-id="35704-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35704-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35704-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35704-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35704-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35704-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35704-107">Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода</span><span class="sxs-lookup"><span data-stu-id="35704-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="35704-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="35704-108">Properties</span></span>
|<span data-ttu-id="35704-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="35704-109">Property</span></span>|<span data-ttu-id="35704-110">Тип</span><span class="sxs-lookup"><span data-stu-id="35704-110">Type</span></span>|<span data-ttu-id="35704-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35704-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35704-112">енроллменттокен</span><span class="sxs-lookup"><span data-stu-id="35704-112">enrollmentToken</span></span>|<span data-ttu-id="35704-113">String</span><span class="sxs-lookup"><span data-stu-id="35704-113">String</span></span>|<span data-ttu-id="35704-114">Маркер регистрации, используемый пользователем для регистрации своего устройства.</span><span class="sxs-lookup"><span data-stu-id="35704-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="35704-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="35704-115">qrCodeContent</span></span>|<span data-ttu-id="35704-116">String</span><span class="sxs-lookup"><span data-stu-id="35704-116">String</span></span>|<span data-ttu-id="35704-117">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="35704-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="35704-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="35704-118">qrCodeImage</span></span>|[<span data-ttu-id="35704-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="35704-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="35704-120">Созданный QR код для маркера.</span><span class="sxs-lookup"><span data-stu-id="35704-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35704-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="35704-121">Relationships</span></span>
<span data-ttu-id="35704-122">Нет</span><span class="sxs-lookup"><span data-stu-id="35704-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35704-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35704-123">JSON Representation</span></span>
<span data-ttu-id="35704-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35704-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```






