---
title: тип enum vppTokenState
description: Возможные состояния, связанные с маркером Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c7addece5e6cf2281e99439c957ceb567a28de73
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790614"
---
# <a name="vpptokenstate-enum-type"></a>тип enum vppTokenState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные состояния, связанные с маркером Apple Volume Purchase Program.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние по умолчанию.|
|допустимо|1|Маркер действителен.|
|истек срок действия|2|Срок действия маркера истек.|
|Недопустимый|3|Маркер недействителен.|
|назначеноToExternalMDM|4 |Маркер управляется другой службой MDM.|
|duplicateLocationId|5 |Маркер связан с тем же расположением, что и другой маркер на учетной записи.|



