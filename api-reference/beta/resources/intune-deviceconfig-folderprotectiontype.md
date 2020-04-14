---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ded583dfe44d393a2ae1c8f56f9952feb85cf857
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444290"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="93220-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="93220-103">folderProtectionType enum type</span></span>

<span data-ttu-id="93220-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93220-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93220-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93220-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93220-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93220-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93220-107">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="93220-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="93220-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="93220-108">Members</span></span>
|<span data-ttu-id="93220-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="93220-109">Member</span></span>|<span data-ttu-id="93220-110">Значение</span><span class="sxs-lookup"><span data-stu-id="93220-110">Value</span></span>|<span data-ttu-id="93220-111">Описание</span><span class="sxs-lookup"><span data-stu-id="93220-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93220-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="93220-112">userDefined</span></span>|<span data-ttu-id="93220-113">нуль</span><span class="sxs-lookup"><span data-stu-id="93220-113">0</span></span>|<span data-ttu-id="93220-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="93220-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="93220-115">подключить</span><span class="sxs-lookup"><span data-stu-id="93220-115">enable</span></span>|<span data-ttu-id="93220-116">1,1</span><span class="sxs-lookup"><span data-stu-id="93220-116">1</span></span>|<span data-ttu-id="93220-117">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="93220-117">Block functionality.</span></span>|
|<span data-ttu-id="93220-118">аудитмоде</span><span class="sxs-lookup"><span data-stu-id="93220-118">auditMode</span></span>|<span data-ttu-id="93220-119">2</span><span class="sxs-lookup"><span data-stu-id="93220-119">2</span></span>|<span data-ttu-id="93220-120">Разрешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="93220-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="93220-121">блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="93220-121">blockDiskModification</span></span>|<span data-ttu-id="93220-122">4</span><span class="sxs-lookup"><span data-stu-id="93220-122">3</span></span>|<span data-ttu-id="93220-123">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="93220-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="93220-124">аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="93220-124">auditDiskModification</span></span>|<span data-ttu-id="93220-125">4 </span><span class="sxs-lookup"><span data-stu-id="93220-125">4</span></span>|<span data-ttu-id="93220-126">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="93220-126">Generate logs when untrusted apps write to disk sectors.</span></span>|



