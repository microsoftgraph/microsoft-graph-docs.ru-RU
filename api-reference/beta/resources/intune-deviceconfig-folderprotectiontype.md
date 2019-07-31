---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: af7c5a9837c0f31401a4a662efdc63e4f6febb8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001350"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="d0459-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="d0459-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="d0459-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0459-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0459-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0459-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0459-106">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="d0459-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="d0459-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d0459-107">Members</span></span>
|<span data-ttu-id="d0459-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d0459-108">Member</span></span>|<span data-ttu-id="d0459-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d0459-109">Value</span></span>|<span data-ttu-id="d0459-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0459-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0459-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="d0459-111">userDefined</span></span>|<span data-ttu-id="d0459-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d0459-112">0</span></span>|<span data-ttu-id="d0459-113">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="d0459-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="d0459-114">подключить</span><span class="sxs-lookup"><span data-stu-id="d0459-114">enable</span></span>|<span data-ttu-id="d0459-115">1,1</span><span class="sxs-lookup"><span data-stu-id="d0459-115">1</span></span>|<span data-ttu-id="d0459-116">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="d0459-116">Block functionality.</span></span>|
|<span data-ttu-id="d0459-117">Аудитмоде</span><span class="sxs-lookup"><span data-stu-id="d0459-117">auditMode</span></span>|<span data-ttu-id="d0459-118">2</span><span class="sxs-lookup"><span data-stu-id="d0459-118">2</span></span>|<span data-ttu-id="d0459-119">Разрешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="d0459-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="d0459-120">Блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="d0459-120">blockDiskModification</span></span>|<span data-ttu-id="d0459-121">4</span><span class="sxs-lookup"><span data-stu-id="d0459-121">3</span></span>|<span data-ttu-id="d0459-122">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="d0459-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="d0459-123">Аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="d0459-123">auditDiskModification</span></span>|<span data-ttu-id="d0459-124">SP4</span><span class="sxs-lookup"><span data-stu-id="d0459-124">4</span></span>|<span data-ttu-id="d0459-125">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="d0459-125">Generate logs when untrusted apps write to disk sectors.</span></span>|





