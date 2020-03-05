---
title: тип перечисления Граупполициконфигуратионтипе
description: Тип конфигурации групповой политики
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6ac65432d389cc0f2fd7696cb7ec6753c3ff76ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528108"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="0db25-103">тип перечисления Граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="0db25-103">groupPolicyConfigurationType enum type</span></span>

<span data-ttu-id="0db25-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0db25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0db25-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0db25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0db25-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0db25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0db25-107">Тип конфигурации групповой политики</span><span class="sxs-lookup"><span data-stu-id="0db25-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="0db25-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0db25-108">Members</span></span>
|<span data-ttu-id="0db25-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0db25-109">Member</span></span>|<span data-ttu-id="0db25-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0db25-110">Value</span></span>|<span data-ttu-id="0db25-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0db25-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db25-112">policy</span><span class="sxs-lookup"><span data-stu-id="0db25-112">policy</span></span>|<span data-ttu-id="0db25-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0db25-113">0</span></span>|<span data-ttu-id="0db25-114">Тип политики не является восстановленным значением, что означает, что значение удаляется, что позволяет использовать исходное значение конфигурации.</span><span class="sxs-lookup"><span data-stu-id="0db25-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="0db25-115">Тип политики заменяется параметром конфигурации приложения, поэтому приложение всегда знает значение.</span><span class="sxs-lookup"><span data-stu-id="0db25-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="0db25-116">Тип политики не позволяет пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="0db25-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="0db25-117">параметров</span><span class="sxs-lookup"><span data-stu-id="0db25-117">preference</span></span>|<span data-ttu-id="0db25-118">1 </span><span class="sxs-lookup"><span data-stu-id="0db25-118">1</span></span>|<span data-ttu-id="0db25-119">Тип предпочтения приводит к восстановлению значения, которое означает, что значение не удаляется из реестра.</span><span class="sxs-lookup"><span data-stu-id="0db25-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="0db25-120">Тип предпочтения перезапишет настраиваемое значение пользователем и не сохранит предыдущее значение.</span><span class="sxs-lookup"><span data-stu-id="0db25-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="0db25-121">Тип предпочтения не запрещает пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="0db25-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|



