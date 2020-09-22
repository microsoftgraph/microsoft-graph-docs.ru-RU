---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ccdaf6625685a0e9e317ad01c8b81fffa04f651
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994073"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="8232e-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="8232e-103">folderProtectionType enum type</span></span>

<span data-ttu-id="8232e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8232e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8232e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8232e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8232e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8232e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8232e-107">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="8232e-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="8232e-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8232e-108">Members</span></span>
|<span data-ttu-id="8232e-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8232e-109">Member</span></span>|<span data-ttu-id="8232e-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8232e-110">Value</span></span>|<span data-ttu-id="8232e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8232e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8232e-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="8232e-112">userDefined</span></span>|<span data-ttu-id="8232e-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8232e-113">0</span></span>|<span data-ttu-id="8232e-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="8232e-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="8232e-115">подключить</span><span class="sxs-lookup"><span data-stu-id="8232e-115">enable</span></span>|<span data-ttu-id="8232e-116">1 </span><span class="sxs-lookup"><span data-stu-id="8232e-116">1</span></span>|<span data-ttu-id="8232e-117">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="8232e-117">Block functionality.</span></span>|
|<span data-ttu-id="8232e-118">аудитмоде</span><span class="sxs-lookup"><span data-stu-id="8232e-118">auditMode</span></span>|<span data-ttu-id="8232e-119">2 </span><span class="sxs-lookup"><span data-stu-id="8232e-119">2</span></span>|<span data-ttu-id="8232e-120">Разрешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="8232e-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="8232e-121">блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="8232e-121">blockDiskModification</span></span>|<span data-ttu-id="8232e-122">4</span><span class="sxs-lookup"><span data-stu-id="8232e-122">3</span></span>|<span data-ttu-id="8232e-123">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="8232e-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="8232e-124">аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="8232e-124">auditDiskModification</span></span>|<span data-ttu-id="8232e-125">4 </span><span class="sxs-lookup"><span data-stu-id="8232e-125">4</span></span>|<span data-ttu-id="8232e-126">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="8232e-126">Generate logs when untrusted apps write to disk sectors.</span></span>|






