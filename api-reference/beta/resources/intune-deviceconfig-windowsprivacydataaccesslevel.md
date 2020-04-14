---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: deebb9f7d24646d18b425b0948eb4a229341fb6d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444059"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="b8da4-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="b8da4-103">windowsPrivacyDataAccessLevel enum type</span></span>

<span data-ttu-id="b8da4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8da4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8da4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8da4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8da4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8da4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8da4-107">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="b8da4-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="b8da4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b8da4-108">Members</span></span>
|<span data-ttu-id="b8da4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b8da4-109">Member</span></span>|<span data-ttu-id="b8da4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b8da4-110">Value</span></span>|<span data-ttu-id="b8da4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8da4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8da4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b8da4-112">notConfigured</span></span>|<span data-ttu-id="b8da4-113">нуль</span><span class="sxs-lookup"><span data-stu-id="b8da4-113">0</span></span>|<span data-ttu-id="b8da4-114">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="b8da4-114">No access level specified, no intents.</span></span> <span data-ttu-id="b8da4-115">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="b8da4-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="b8da4-116">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="b8da4-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="b8da4-117">форцеаллов</span><span class="sxs-lookup"><span data-stu-id="b8da4-117">forceAllow</span></span>|<span data-ttu-id="b8da4-118">1,1</span><span class="sxs-lookup"><span data-stu-id="b8da4-118">1</span></span>|<span data-ttu-id="b8da4-119">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b8da4-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="b8da4-120">форцедени</span><span class="sxs-lookup"><span data-stu-id="b8da4-120">forceDeny</span></span>|<span data-ttu-id="b8da4-121">2</span><span class="sxs-lookup"><span data-stu-id="b8da4-121">2</span></span>|<span data-ttu-id="b8da4-122">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b8da4-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="b8da4-123">усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="b8da4-123">userInControl</span></span>|<span data-ttu-id="b8da4-124">4</span><span class="sxs-lookup"><span data-stu-id="b8da4-124">3</span></span>|<span data-ttu-id="b8da4-125">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b8da4-125">Users will be prompted when apps try to access specified privacy data.</span></span>|



