---
ms.localizationpriority: medium
ms.openlocfilehash: 48b73a117c130f786a72bbc554632b0a858ebab7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289664"
---
<!-- markdownlint-disable MD041-->

Когда приложение запрашивает связь, возвращающую коллекцию типов directoryObject, но у него нет разрешения на чтение определенного производного типа (например, устройства), элементы этого типа возвращаются, но с ограниченными сведениями. С помощью этого поведения приложения могут запрашивать минимальные разрешения, которые им требуются, а не использовать набор разрешений *Directory.** Сведения см. в разделе [Ограниченные сведения, возвращаемые для недоступных объектов member](/graph/permissions-reference#limited-information-returned-for-inaccessible-member-objects).
