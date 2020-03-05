---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 23717d1e798059f1ca025a3f80279804b616b17f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529987"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="91f08-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="91f08-103">folderProtectionType enum type</span></span>

<span data-ttu-id="91f08-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="91f08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91f08-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91f08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91f08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91f08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91f08-107">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="91f08-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="91f08-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="91f08-108">Members</span></span>
|<span data-ttu-id="91f08-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="91f08-109">Member</span></span>|<span data-ttu-id="91f08-110">Значение</span><span class="sxs-lookup"><span data-stu-id="91f08-110">Value</span></span>|<span data-ttu-id="91f08-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91f08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91f08-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="91f08-112">userDefined</span></span>|<span data-ttu-id="91f08-113">нуль</span><span class="sxs-lookup"><span data-stu-id="91f08-113">0</span></span>|<span data-ttu-id="91f08-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="91f08-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="91f08-115">подключить</span><span class="sxs-lookup"><span data-stu-id="91f08-115">enable</span></span>|<span data-ttu-id="91f08-116">1 </span><span class="sxs-lookup"><span data-stu-id="91f08-116">1</span></span>|<span data-ttu-id="91f08-117">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="91f08-117">Block functionality.</span></span>|
|<span data-ttu-id="91f08-118">аудитмоде</span><span class="sxs-lookup"><span data-stu-id="91f08-118">auditMode</span></span>|<span data-ttu-id="91f08-119">2 </span><span class="sxs-lookup"><span data-stu-id="91f08-119">2</span></span>|<span data-ttu-id="91f08-120">Разрешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="91f08-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="91f08-121">блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="91f08-121">blockDiskModification</span></span>|<span data-ttu-id="91f08-122">3 </span><span class="sxs-lookup"><span data-stu-id="91f08-122">3</span></span>|<span data-ttu-id="91f08-123">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="91f08-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="91f08-124">аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="91f08-124">auditDiskModification</span></span>|<span data-ttu-id="91f08-125">4 </span><span class="sxs-lookup"><span data-stu-id="91f08-125">4</span></span>|<span data-ttu-id="91f08-126">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="91f08-126">Generate logs when untrusted apps write to disk sectors.</span></span>|



