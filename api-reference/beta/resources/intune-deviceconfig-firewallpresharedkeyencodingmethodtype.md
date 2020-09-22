---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4d82b9ec0e18a73db9cd4564efff7fd36dd7cda9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994087"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="1235c-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="1235c-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="1235c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1235c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1235c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1235c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1235c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1235c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1235c-107">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="1235c-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="1235c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="1235c-108">Members</span></span>
|<span data-ttu-id="1235c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="1235c-109">Member</span></span>|<span data-ttu-id="1235c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="1235c-110">Value</span></span>|<span data-ttu-id="1235c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1235c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1235c-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="1235c-112">deviceDefault</span></span>|<span data-ttu-id="1235c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="1235c-113">0</span></span>|<span data-ttu-id="1235c-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="1235c-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1235c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="1235c-115">none</span></span>|<span data-ttu-id="1235c-116">1 </span><span class="sxs-lookup"><span data-stu-id="1235c-116">1</span></span>|<span data-ttu-id="1235c-117">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="1235c-117">Preshared key is not encoded.</span></span> <span data-ttu-id="1235c-118">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="1235c-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="1235c-119">utF8</span><span class="sxs-lookup"><span data-stu-id="1235c-119">utF8</span></span>|<span data-ttu-id="1235c-120">2 </span><span class="sxs-lookup"><span data-stu-id="1235c-120">2</span></span>|<span data-ttu-id="1235c-121">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="1235c-121">Encode the preshared key using UTF-8</span></span>|






