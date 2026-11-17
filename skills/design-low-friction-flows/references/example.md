# 完整案例 / Worked example

**输入。** 员工已上传申请材料，预览页提示有一张附件模糊。有的申请只有一张，有的有多张。历史方案让人返回列表重新上传全部文件。

**推荐交互。** 保留预览与已填表单。失败附件旁显示「这张看不清，请换一张」，并提供「替换」。如果系统能定位到一项，按钮直接指向该附件。只有多个可疑目标且无法定位时，列出文件名与缩略图，请用户选要换的那张。

**状态与失败。** 选新文件后先上传。新文件成功时才更新附件并重新校验该项。上传失败保留旧附件和其他表单内容，在原位置显示「上传失败，请重试」。替换前用户可以离开，返回时继续处理同一草稿。只有附件确实为必交材料时才阻止提交。

**走查。** 单附件模糊，用户从原位换图。多附件且目标不明，用户只选一次。替换失败，原附件仍在且其他输入完整。无材料要求的申请可按既有规则提交。

---

**Input.** A preview warns that an attachment in an application is unreadable. Some drafts have one file and others have several. The old flow sends the user back to the list and requires a full re-upload.

**Recommended flow.** Keep the preview and existing form inputs. Put “This image is hard to read. Replace it.” next to the failed attachment. When a file is identifiable, target it directly. For multiple ambiguous candidates, offer filenames and thumbnails and ask the user to choose the one to replace.

**State and recovery.** Upload the replacement first. Swap and revalidate it only after upload succeeds. On failure, preserve the old file and other inputs and show “Upload failed. Try again” in place. Let the user leave and resume the same draft. Block submission only if the file is required by the underlying process.

**Walkthrough.** A single unreadable file is replaced in place. With multiple ambiguous files, the user chooses once. A failed upload preserves the original file and other inputs. Requests with no attachment requirement can still submit under the existing rule.
