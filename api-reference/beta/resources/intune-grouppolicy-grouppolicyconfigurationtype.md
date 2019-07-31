---
title: тип перечисления Граупполициконфигуратионтипе
description: Тип конфигурации групповой политики
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6e0e7f2b1a9c7817af614c2753e4e5fcfe0fe2c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011010"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="face7-103">тип перечисления Граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="face7-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="face7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="face7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="face7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="face7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="face7-106">Тип конфигурации групповой политики</span><span class="sxs-lookup"><span data-stu-id="face7-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="face7-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="face7-107">Members</span></span>
|<span data-ttu-id="face7-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="face7-108">Member</span></span>|<span data-ttu-id="face7-109">Значение</span><span class="sxs-lookup"><span data-stu-id="face7-109">Value</span></span>|<span data-ttu-id="face7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="face7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="face7-111">policy</span><span class="sxs-lookup"><span data-stu-id="face7-111">policy</span></span>|<span data-ttu-id="face7-112">нуль</span><span class="sxs-lookup"><span data-stu-id="face7-112">0</span></span>|<span data-ttu-id="face7-113">Тип политики не является восстановленным значением, что означает, что значение удаляется, что позволяет использовать исходное значение конфигурации.</span><span class="sxs-lookup"><span data-stu-id="face7-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="face7-114">Тип политики заменяется параметром конфигурации приложения, поэтому приложение всегда знает значение.</span><span class="sxs-lookup"><span data-stu-id="face7-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="face7-115">Тип политики не позволяет пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="face7-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="face7-116">параметров</span><span class="sxs-lookup"><span data-stu-id="face7-116">preference</span></span>|<span data-ttu-id="face7-117">1,1</span><span class="sxs-lookup"><span data-stu-id="face7-117">1</span></span>|<span data-ttu-id="face7-118">Тип предпочтения приводит к восстановлению значения, которое означает, что значение не удаляется из реестра.</span><span class="sxs-lookup"><span data-stu-id="face7-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="face7-119">Тип предпочтения перезапишет настраиваемое значение пользователем и не сохранит предыдущее значение.</span><span class="sxs-lookup"><span data-stu-id="face7-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="face7-120">Тип предпочтения не запрещает пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="face7-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|





