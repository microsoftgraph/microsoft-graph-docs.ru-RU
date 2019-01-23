---
title: Тип ресурса androidEnrollmentCompanyCode
description: Класс для хранения данных регистрации специальные, используемые на выдачу через компании Google Android API для управления, такие как маркер, URL-адрес и QR кода содержимого
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be5b2a94445e95fe18271467b6661320d8204d76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430609"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="07f6f-103">Тип ресурса androidEnrollmentCompanyCode</span><span class="sxs-lookup"><span data-stu-id="07f6f-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="07f6f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07f6f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07f6f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07f6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07f6f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07f6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f6f-107">Класс для хранения данных регистрации специальные, используемые на выдачу через компании Google Android API для управления, такие как маркер, URL-адрес и QR кода содержимого</span><span class="sxs-lookup"><span data-stu-id="07f6f-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="07f6f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07f6f-108">Properties</span></span>
|<span data-ttu-id="07f6f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07f6f-109">Property</span></span>|<span data-ttu-id="07f6f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07f6f-110">Type</span></span>|<span data-ttu-id="07f6f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07f6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07f6f-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="07f6f-112">enrollmentToken</span></span>|<span data-ttu-id="07f6f-113">String</span><span class="sxs-lookup"><span data-stu-id="07f6f-113">String</span></span>|<span data-ttu-id="07f6f-114">Регистрации маркер, используемый пользователем, чтобы зарегистрировать свое устройство.</span><span class="sxs-lookup"><span data-stu-id="07f6f-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="07f6f-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="07f6f-115">qrCodeContent</span></span>|<span data-ttu-id="07f6f-116">String</span><span class="sxs-lookup"><span data-stu-id="07f6f-116">String</span></span>|<span data-ttu-id="07f6f-117">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="07f6f-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="07f6f-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="07f6f-118">qrCodeImage</span></span>|[<span data-ttu-id="07f6f-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="07f6f-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="07f6f-120">Созданный код QR для маркера.</span><span class="sxs-lookup"><span data-stu-id="07f6f-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07f6f-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="07f6f-121">Relationships</span></span>
<span data-ttu-id="07f6f-122">Нет</span><span class="sxs-lookup"><span data-stu-id="07f6f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07f6f-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07f6f-123">JSON Representation</span></span>
<span data-ttu-id="07f6f-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07f6f-124">Here is a JSON representation of the resource.</span></span>
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




