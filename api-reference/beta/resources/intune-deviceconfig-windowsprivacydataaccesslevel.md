---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 44ac906a390aff82e4399181014628725673b1b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000265"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="4dbe1-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="4dbe1-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="4dbe1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dbe1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dbe1-106">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-106">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="4dbe1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="4dbe1-107">Members</span></span>
|<span data-ttu-id="4dbe1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="4dbe1-108">Member</span></span>|<span data-ttu-id="4dbe1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="4dbe1-109">Value</span></span>|<span data-ttu-id="4dbe1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4dbe1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dbe1-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4dbe1-111">notConfigured</span></span>|<span data-ttu-id="4dbe1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="4dbe1-112">0</span></span>|<span data-ttu-id="4dbe1-113">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-113">No access level specified, no intents.</span></span> <span data-ttu-id="4dbe1-114">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-114">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="4dbe1-115">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-115">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="4dbe1-116">Форцеаллов</span><span class="sxs-lookup"><span data-stu-id="4dbe1-116">forceAllow</span></span>|<span data-ttu-id="4dbe1-117">1,1</span><span class="sxs-lookup"><span data-stu-id="4dbe1-117">1</span></span>|<span data-ttu-id="4dbe1-118">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-118">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="4dbe1-119">Форцедени</span><span class="sxs-lookup"><span data-stu-id="4dbe1-119">forceDeny</span></span>|<span data-ttu-id="4dbe1-120">2</span><span class="sxs-lookup"><span data-stu-id="4dbe1-120">2</span></span>|<span data-ttu-id="4dbe1-121">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-121">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="4dbe1-122">Усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="4dbe1-122">userInControl</span></span>|<span data-ttu-id="4dbe1-123">4</span><span class="sxs-lookup"><span data-stu-id="4dbe1-123">3</span></span>|<span data-ttu-id="4dbe1-124">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4dbe1-124">Users will be prompted when apps try to access specified privacy data.</span></span>|





