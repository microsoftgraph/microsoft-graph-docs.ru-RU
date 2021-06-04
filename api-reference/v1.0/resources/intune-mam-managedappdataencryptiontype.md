---
title: тип enum managedAppDataEncryptionType
description: Представляет уровень шифрования данных приложений для управляемых приложений
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a3cbe74f8dbc81330b899b4acedcbc880b8d81d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754499"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="6535c-103">тип enum managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="6535c-103">managedAppDataEncryptionType enum type</span></span>

<span data-ttu-id="6535c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6535c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6535c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6535c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6535c-106">Представляет уровень шифрования данных приложений для управляемых приложений</span><span class="sxs-lookup"><span data-stu-id="6535c-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="6535c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6535c-107">Members</span></span>
|<span data-ttu-id="6535c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6535c-108">Member</span></span>|<span data-ttu-id="6535c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6535c-109">Value</span></span>|<span data-ttu-id="6535c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6535c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6535c-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="6535c-111">useDeviceSettings</span></span>|<span data-ttu-id="6535c-112">0</span><span class="sxs-lookup"><span data-stu-id="6535c-112">0</span></span>|<span data-ttu-id="6535c-113">Данные приложения шифруются в зависимости от параметров по умолчанию на устройстве.</span><span class="sxs-lookup"><span data-stu-id="6535c-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="6535c-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="6535c-114">afterDeviceRestart</span></span>|<span data-ttu-id="6535c-115">1</span><span class="sxs-lookup"><span data-stu-id="6535c-115">1</span></span>|<span data-ttu-id="6535c-116">Данные приложения шифруются при перезапуске устройства.</span><span class="sxs-lookup"><span data-stu-id="6535c-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="6535c-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="6535c-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="6535c-118">2</span><span class="sxs-lookup"><span data-stu-id="6535c-118">2</span></span>|<span data-ttu-id="6535c-119">Данные приложения, связанные с этой политикой, шифруются при блокировке устройства, за исключением открытых файлов.</span><span class="sxs-lookup"><span data-stu-id="6535c-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="6535c-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6535c-120">whenDeviceLocked</span></span>|<span data-ttu-id="6535c-121">3</span><span class="sxs-lookup"><span data-stu-id="6535c-121">3</span></span>|<span data-ttu-id="6535c-122">Данные приложения, связанные с этой политикой, шифруются при блокировке устройства</span><span class="sxs-lookup"><span data-stu-id="6535c-122">App data associated with this policy is encrypted when the device is locked</span></span>|




