---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: tfitzmac
ms.openlocfilehash: 15de11384195350b455cd4696a260aedf1de7a26
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354036"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="38279-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="38279-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="38279-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38279-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38279-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38279-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38279-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="38279-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38279-107">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="38279-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="38279-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="38279-108">Properties</span></span>
|<span data-ttu-id="38279-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="38279-109">Property</span></span>|<span data-ttu-id="38279-110">Тип</span><span class="sxs-lookup"><span data-stu-id="38279-110">Type</span></span>|<span data-ttu-id="38279-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38279-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38279-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="38279-112">encryptionMethod</span></span>|[<span data-ttu-id="38279-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="38279-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="38279-114">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="38279-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="38279-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="38279-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="38279-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="38279-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="38279-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="38279-117">Boolean</span></span>|<span data-ttu-id="38279-118">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="38279-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="38279-119">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="38279-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="38279-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="38279-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="38279-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="38279-121">Boolean</span></span>|<span data-ttu-id="38279-122">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="38279-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38279-123">Связи</span><span class="sxs-lookup"><span data-stu-id="38279-123">Relationships</span></span>
<span data-ttu-id="38279-124">Нет</span><span class="sxs-lookup"><span data-stu-id="38279-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38279-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38279-125">JSON Representation</span></span>
<span data-ttu-id="38279-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38279-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```





