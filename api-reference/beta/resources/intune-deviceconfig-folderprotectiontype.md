---
title: тип перечисления Фолдерпротектионтипе
description: Возможные значения защиты папок
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 36ddb339db6710006a90e78b6f8eb2d298877077
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49198869"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="53141-103">тип перечисления Фолдерпротектионтипе</span><span class="sxs-lookup"><span data-stu-id="53141-103">folderProtectionType enum type</span></span>

<span data-ttu-id="53141-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53141-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53141-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53141-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53141-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53141-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53141-107">Возможные значения защиты папок</span><span class="sxs-lookup"><span data-stu-id="53141-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="53141-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="53141-108">Members</span></span>
|<span data-ttu-id="53141-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="53141-109">Member</span></span>|<span data-ttu-id="53141-110">Значение</span><span class="sxs-lookup"><span data-stu-id="53141-110">Value</span></span>|<span data-ttu-id="53141-111">Описание</span><span class="sxs-lookup"><span data-stu-id="53141-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53141-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="53141-112">userDefined</span></span>|<span data-ttu-id="53141-113">нуль</span><span class="sxs-lookup"><span data-stu-id="53141-113">0</span></span>|<span data-ttu-id="53141-114">Значение по умолчанию для устройства, без намерения.</span><span class="sxs-lookup"><span data-stu-id="53141-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="53141-115">подключить</span><span class="sxs-lookup"><span data-stu-id="53141-115">enable</span></span>|<span data-ttu-id="53141-116">1,1</span><span class="sxs-lookup"><span data-stu-id="53141-116">1</span></span>|<span data-ttu-id="53141-117">Функциональная возможность блока.</span><span class="sxs-lookup"><span data-stu-id="53141-117">Block functionality.</span></span>|
|<span data-ttu-id="53141-118">аудитмоде</span><span class="sxs-lookup"><span data-stu-id="53141-118">auditMode</span></span>|<span data-ttu-id="53141-119">2</span><span class="sxs-lookup"><span data-stu-id="53141-119">2</span></span>|<span data-ttu-id="53141-120">Разрешите функциональные возможности, но Создайте журналы.</span><span class="sxs-lookup"><span data-stu-id="53141-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="53141-121">блоккдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="53141-121">blockDiskModification</span></span>|<span data-ttu-id="53141-122">4</span><span class="sxs-lookup"><span data-stu-id="53141-122">3</span></span>|<span data-ttu-id="53141-123">Блокировать запись недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="53141-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="53141-124">аудитдискмодификатион</span><span class="sxs-lookup"><span data-stu-id="53141-124">auditDiskModification</span></span>|<span data-ttu-id="53141-125">4 </span><span class="sxs-lookup"><span data-stu-id="53141-125">4</span></span>|<span data-ttu-id="53141-126">Создание журналов при записи недоверенных приложений в секторах диска.</span><span class="sxs-lookup"><span data-stu-id="53141-126">Generate logs when untrusted apps write to disk sectors.</span></span>|




