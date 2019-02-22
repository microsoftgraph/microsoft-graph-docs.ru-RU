---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2cdf124d3da6bf2c08954365a87ae0a97b05267
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159068"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="ef823-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="ef823-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="ef823-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef823-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef823-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef823-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef823-106">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="ef823-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="ef823-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ef823-107">Members</span></span>
|<span data-ttu-id="ef823-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ef823-108">Member</span></span>|<span data-ttu-id="ef823-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ef823-109">Value</span></span>|<span data-ttu-id="ef823-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef823-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef823-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ef823-111">notConfigured</span></span>|<span data-ttu-id="ef823-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ef823-112">0</span></span>|<span data-ttu-id="ef823-113">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="ef823-113">No access level specified, no intents.</span></span> <span data-ttu-id="ef823-114">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="ef823-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="ef823-115">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="ef823-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="ef823-116">Форцеаллов</span><span class="sxs-lookup"><span data-stu-id="ef823-116">forceAllow</span></span>|<span data-ttu-id="ef823-117">1,1</span><span class="sxs-lookup"><span data-stu-id="ef823-117">1</span></span>|<span data-ttu-id="ef823-118">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ef823-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="ef823-119">Форцедени</span><span class="sxs-lookup"><span data-stu-id="ef823-119">forceDeny</span></span>|<span data-ttu-id="ef823-120">2</span><span class="sxs-lookup"><span data-stu-id="ef823-120">2</span></span>|<span data-ttu-id="ef823-121">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ef823-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="ef823-122">Усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="ef823-122">userInControl</span></span>|<span data-ttu-id="ef823-123">4</span><span class="sxs-lookup"><span data-stu-id="ef823-123">3</span></span>|<span data-ttu-id="ef823-124">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ef823-124">Users will be prompted when apps try to access specified privacy data.</span></span>|




