---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bba6033985f2b960a272134614d98acc7203a9d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871752"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="575cc-103">Тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="575cc-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="575cc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="575cc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="575cc-105">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="575cc-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="575cc-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="575cc-106">Members</span></span>
|<span data-ttu-id="575cc-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="575cc-107">Member</span></span>|<span data-ttu-id="575cc-108">Значение</span><span class="sxs-lookup"><span data-stu-id="575cc-108">Value</span></span>|<span data-ttu-id="575cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="575cc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="575cc-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="575cc-110">deviceDefault</span></span>|<span data-ttu-id="575cc-111">0</span><span class="sxs-lookup"><span data-stu-id="575cc-111">0</span></span>|<span data-ttu-id="575cc-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="575cc-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="575cc-113">Нет</span><span class="sxs-lookup"><span data-stu-id="575cc-113">none</span></span>|<span data-ttu-id="575cc-114">1</span><span class="sxs-lookup"><span data-stu-id="575cc-114">1</span></span>|<span data-ttu-id="575cc-115">Предварительный ключ не кодируются.</span><span class="sxs-lookup"><span data-stu-id="575cc-115">Preshared key is not encoded.</span></span> <span data-ttu-id="575cc-116">Вместо этого он будет храниться в формате Юникода</span><span class="sxs-lookup"><span data-stu-id="575cc-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="575cc-117">utF8</span><span class="sxs-lookup"><span data-stu-id="575cc-117">utF8</span></span>|<span data-ttu-id="575cc-118">2</span><span class="sxs-lookup"><span data-stu-id="575cc-118">2</span></span>|<span data-ttu-id="575cc-119">Кодирование предварительный ключ, используя UTF-8</span><span class="sxs-lookup"><span data-stu-id="575cc-119">Encode the preshared key using UTF-8</span></span>|



