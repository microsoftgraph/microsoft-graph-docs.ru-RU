---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc508f3feaf1353d83a87cd0403f9ede2bbcad13
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730488"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="581d3-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="581d3-103">folderProtectionType enum type</span></span>

<span data-ttu-id="581d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="581d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="581d3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="581d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="581d3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="581d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="581d3-107">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="581d3-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="581d3-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="581d3-108">Members</span></span>
|<span data-ttu-id="581d3-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="581d3-109">Member</span></span>|<span data-ttu-id="581d3-110">Значение</span><span class="sxs-lookup"><span data-stu-id="581d3-110">Value</span></span>|<span data-ttu-id="581d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="581d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581d3-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="581d3-112">userDefined</span></span>|<span data-ttu-id="581d3-113">нуль</span><span class="sxs-lookup"><span data-stu-id="581d3-113">0</span></span>|<span data-ttu-id="581d3-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="581d3-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="581d3-115">подключить</span><span class="sxs-lookup"><span data-stu-id="581d3-115">enable</span></span>|<span data-ttu-id="581d3-116">1,1</span><span class="sxs-lookup"><span data-stu-id="581d3-116">1</span></span>|<span data-ttu-id="581d3-117">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="581d3-117">Block functionality.</span></span>|
|<span data-ttu-id="581d3-118">аудитмоде</span><span class="sxs-lookup"><span data-stu-id="581d3-118">auditMode</span></span>|<span data-ttu-id="581d3-119">2</span><span class="sxs-lookup"><span data-stu-id="581d3-119">2</span></span>|<span data-ttu-id="581d3-120">Разрешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="581d3-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="581d3-121">блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="581d3-121">blockDiskModification</span></span>|<span data-ttu-id="581d3-122">4</span><span class="sxs-lookup"><span data-stu-id="581d3-122">3</span></span>|<span data-ttu-id="581d3-123">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="581d3-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="581d3-124">аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="581d3-124">auditDiskModification</span></span>|<span data-ttu-id="581d3-125">4 </span><span class="sxs-lookup"><span data-stu-id="581d3-125">4</span></span>|<span data-ttu-id="581d3-126">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="581d3-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





