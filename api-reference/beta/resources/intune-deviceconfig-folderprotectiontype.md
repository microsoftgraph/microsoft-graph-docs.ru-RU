---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a8242f361f68ec7e295950ea29e7478de414ad6b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791739"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="d9568-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d9568-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="d9568-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9568-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9568-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9568-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9568-106">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="d9568-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="d9568-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d9568-107">Members</span></span>
|<span data-ttu-id="d9568-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d9568-108">Member</span></span>|<span data-ttu-id="d9568-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d9568-109">Value</span></span>|<span data-ttu-id="d9568-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d9568-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9568-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="d9568-111">userDefined</span></span>|<span data-ttu-id="d9568-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d9568-112">0</span></span>|<span data-ttu-id="d9568-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="d9568-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="d9568-114">подключить</span><span class="sxs-lookup"><span data-stu-id="d9568-114">enable</span></span>|<span data-ttu-id="d9568-115">1,1</span><span class="sxs-lookup"><span data-stu-id="d9568-115">1</span></span>|<span data-ttu-id="d9568-116">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="d9568-116">Block functionality.</span></span>|
|<span data-ttu-id="d9568-117">аудитмоде</span><span class="sxs-lookup"><span data-stu-id="d9568-117">auditMode</span></span>|<span data-ttu-id="d9568-118">2</span><span class="sxs-lookup"><span data-stu-id="d9568-118">2</span></span>|<span data-ttu-id="d9568-119">Разрешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="d9568-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="d9568-120">блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="d9568-120">blockDiskModification</span></span>|<span data-ttu-id="d9568-121">4</span><span class="sxs-lookup"><span data-stu-id="d9568-121">3</span></span>|<span data-ttu-id="d9568-122">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="d9568-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="d9568-123">аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="d9568-123">auditDiskModification</span></span>|<span data-ttu-id="d9568-124">4 </span><span class="sxs-lookup"><span data-stu-id="d9568-124">4</span></span>|<span data-ttu-id="d9568-125">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="d9568-125">Generate logs when untrusted apps write to disk sectors.</span></span>|



