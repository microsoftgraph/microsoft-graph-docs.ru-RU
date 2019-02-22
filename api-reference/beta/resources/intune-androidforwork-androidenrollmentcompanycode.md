---
title: Тип ресурса Андроиденроллменткомпаникоде
description: Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0cd3ede4193ea3fdb33d33010349812150848e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169344"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="3d32d-103">Тип ресурса Андроиденроллменткомпаникоде</span><span class="sxs-lookup"><span data-stu-id="3d32d-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="3d32d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d32d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d32d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d32d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d32d-106">Класс для хранения специализированных регистрационных данных, используемых для регистрации через API управления Android для Google, таких как маркер, URL-адрес и содержимое QR-кода</span><span class="sxs-lookup"><span data-stu-id="3d32d-106">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="3d32d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d32d-107">Properties</span></span>
|<span data-ttu-id="3d32d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d32d-108">Property</span></span>|<span data-ttu-id="3d32d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3d32d-109">Type</span></span>|<span data-ttu-id="3d32d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3d32d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d32d-111">Енроллменттокен</span><span class="sxs-lookup"><span data-stu-id="3d32d-111">enrollmentToken</span></span>|<span data-ttu-id="3d32d-112">String</span><span class="sxs-lookup"><span data-stu-id="3d32d-112">String</span></span>|<span data-ttu-id="3d32d-113">Маркер регистрации, используемый пользователем для регистрации своего устройства.</span><span class="sxs-lookup"><span data-stu-id="3d32d-113">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="3d32d-114">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="3d32d-114">qrCodeContent</span></span>|<span data-ttu-id="3d32d-115">String</span><span class="sxs-lookup"><span data-stu-id="3d32d-115">String</span></span>|<span data-ttu-id="3d32d-116">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="3d32d-116">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="3d32d-117">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="3d32d-117">qrCodeImage</span></span>|[<span data-ttu-id="3d32d-118">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3d32d-118">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3d32d-119">Созданный QR код для маркера.</span><span class="sxs-lookup"><span data-stu-id="3d32d-119">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d32d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="3d32d-120">Relationships</span></span>
<span data-ttu-id="3d32d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3d32d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d32d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d32d-122">JSON Representation</span></span>
<span data-ttu-id="3d32d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d32d-123">Here is a JSON representation of the resource.</span></span>
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




