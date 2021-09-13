---
title: тип enum vppTokenState
description: Возможные состояния, связанные с маркером Apple Volume Purchase Program.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a72b2be5a0ce4ff690e05c863cc7faad7023d0e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101165"
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



