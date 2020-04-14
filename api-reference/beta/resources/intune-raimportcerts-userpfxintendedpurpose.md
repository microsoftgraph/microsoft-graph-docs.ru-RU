---
title: тип перечисления Усерпфксинтендедпурпосе
description: Поддерживаемые значения для назначения сертификата пользователя PFX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fb7ee28f73762ec3db6bca213ea1d9e21b4353ce
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462356"
---
# <a name="userpfxintendedpurpose-enum-type"></a><span data-ttu-id="c61f2-103">тип перечисления Усерпфксинтендедпурпосе</span><span class="sxs-lookup"><span data-stu-id="c61f2-103">userPfxIntendedPurpose enum type</span></span>

<span data-ttu-id="c61f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c61f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c61f2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c61f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c61f2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c61f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c61f2-107">Поддерживаемые значения для назначения сертификата пользователя PFX.</span><span class="sxs-lookup"><span data-stu-id="c61f2-107">Supported values for the intended purpose of a user PFX certificate.</span></span>

## <a name="members"></a><span data-ttu-id="c61f2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c61f2-108">Members</span></span>
|<span data-ttu-id="c61f2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c61f2-109">Member</span></span>|<span data-ttu-id="c61f2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c61f2-110">Value</span></span>|<span data-ttu-id="c61f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c61f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c61f2-112">неназначенных</span><span class="sxs-lookup"><span data-stu-id="c61f2-112">unassigned</span></span>|<span data-ttu-id="c61f2-113">нуль</span><span class="sxs-lookup"><span data-stu-id="c61f2-113">0</span></span>|<span data-ttu-id="c61f2-114">Не назначены роли и использования.</span><span class="sxs-lookup"><span data-stu-id="c61f2-114">No roles/usages assigned.</span></span>|
|<span data-ttu-id="c61f2-115">смиминкриптион</span><span class="sxs-lookup"><span data-stu-id="c61f2-115">smimeEncryption</span></span>|<span data-ttu-id="c61f2-116">1,1</span><span class="sxs-lookup"><span data-stu-id="c61f2-116">1</span></span>|<span data-ttu-id="c61f2-117">Является допустимым для шифрования S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c61f2-117">Valid for S/MIME encryption.</span></span>|
|<span data-ttu-id="c61f2-118">смимесигнинг</span><span class="sxs-lookup"><span data-stu-id="c61f2-118">smimeSigning</span></span>|<span data-ttu-id="c61f2-119">2</span><span class="sxs-lookup"><span data-stu-id="c61f2-119">2</span></span>|<span data-ttu-id="c61f2-120">Является допустимым для подписывания S/MIME.</span><span class="sxs-lookup"><span data-stu-id="c61f2-120">Valid for S/MIME signing.</span></span>|
|<span data-ttu-id="c61f2-121">виртуального</span><span class="sxs-lookup"><span data-stu-id="c61f2-121">vpn</span></span>|<span data-ttu-id="c61f2-122">4 </span><span class="sxs-lookup"><span data-stu-id="c61f2-122">4</span></span>|<span data-ttu-id="c61f2-123">Допустимо для использования в VPN.</span><span class="sxs-lookup"><span data-stu-id="c61f2-123">Valid for use in VPN.</span></span>|
|<span data-ttu-id="c61f2-124">подключений</span><span class="sxs-lookup"><span data-stu-id="c61f2-124">wifi</span></span>|<span data-ttu-id="c61f2-125">8 </span><span class="sxs-lookup"><span data-stu-id="c61f2-125">8</span></span>|<span data-ttu-id="c61f2-126">Допустимо для использования в Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="c61f2-126">Valid for use in WiFi.</span></span>|



